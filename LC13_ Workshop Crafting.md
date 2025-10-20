# **Weaponry Material Grid Crafting System**

---

## **System Overview**

The **Weaponry Grid Crafting System** is a unique crafting mechanic where players navigate a "**focus point**" through a coordinate grid using weaponry materials to reach weapon coordinates and craft city weapons. The system creates a strategic resource management challenge where material properties determine movement patterns.

---

## **Core Mechanics**

### **1\. The Grid**

* **Infinite 2D coordinate system** with origin at (0, 0\)  
* **Focus Point**: Current position marker that starts at (0, 0\)  
* **Weapon Coordinates**: Fixed positions on the grid where weapons can be crafted  
* **Influence Radius**: Each weapon has a circular area where it can be crafted

### **2\. Movement System**

Materials move the focus point based on their properties:

#### **Material Properties**

* **Rarity** (0-4+): Determines movement distance

  * 0 (Crude): 1-2 units  
  * 1 (Common): 3-5 units  
  * 2 (Refined): 6-10 units  
  * 3 (Exceptional): 11-20 units  
  * 4+ (Legendary): 21-40 units  
* **Damage Type**: Determines movement direction/pattern

  * **RED**: Cardinal directions (N/S/E/W)  
  * **WHITE**: Diagonal directions (NE/NW/SE/SW)  
  * **BLACK**: Diagonal/Cardinal movement (N/S/E/W/NE/NW/SE/SW)  
  * **PALE**: Teleport to location within range (player choice)  
* **Density**: Modifies movement behavior

  * **Lightweight**: \+25% distance  
  * **Normal**: Standard distance  
  * **Heavy**: \-50% distance. When landing in multiple weapon radii, gain the ability to pick a specific weapon.

### **3\. Weapon Placement Algorithm**

The algorithm is adjusted based on weapon density per rarity. More weapons in a rarity result in a smaller radius to prevent overlap, and distance ranges are expanded for crowded rarities to ensure at least 2 units of spacing.

* **Rarity 0** (46 weapons): Distance 5-25, Radius 6-10  
* **Rarity 1** (19 weapons): Distance 20-40, Radius 8-12  
* **Rarity 2** (65 weapons): Distance 35-65, Radius 6-8  
* **Rarity 3** (12 weapons): Distance 55-85, Radius 6-8  
* **Rarity 4** (3 weapons): Distance 75-105, Radius 4-6

**Note**: The high weapon count in Rarity 2 requires the largest distance range to prevent coordinate clustering.

### **4\. Crafting Process**

1. Player starts at (0, 0).  
2. Uses materials to move the focus point.  
3. After using at least 1 material, the system checks if the focus point is within any weapon radius.  
4. If within radius:  
   * **Single weapon**: That weapon is crafted.  
   * **Multiple weapons**: A random selection occurs.  
5. Focus point resets to (0, 0).

---

## **Visual Example**

       \[R3:6\]  
          \*  
   
\[R2:8\]         \[R2:12\]  
      \*                 \*  
   
            F(0,0)  
   
\[R1: 10\]         \[R1: 8\]  
      \*                  \*  
   
        \[R0:10\]  
          \*

**Legend**:

* **F** \= Focus Point  
* **\*** \= Weapon Coordinate  
* **\[Rn:r\]** \= Rarity 'n' weapon with radius 'r'

---

## **Weaponry Disassembler**

The weaponry disassembler converts existing weapons into **weapon shards** used for grid navigation.

### **Operation**

1. **Load Weapons**: Insert weaponry into the disassembler (accepts /obj/item/ego\_weapon).  
2. **Activate**: Use harm intent on the machine to begin processing.  
3. **Processing**: The machine takes 5 seconds to disassemble all loaded weapons.  
4. **Output**: Each weapon produces 4-7 weapon shards.

### **Shard Property Generation**

Each weapon shard inherits properties from the disassembled weapon:

#### **Rarity Calculation**

Shard Rarity \= (Sum of all attribute requirements / Number of requirements) / 30

* Weapons with no requirements → Rarity 0 (Crude)  
* Average 30 requirements → Rarity 1 (Common)  
* Average 60 requirements → Rarity 2 (Refined)  
* Average 90 requirements → Rarity 3 (Exceptional)  
* Average 120+ requirements → Rarity 4+ (Legendary)

#### **Density Mapping**

Based on weapon attack speed:

* Attack Speed \&lt; 0.7 → "**lightweight**" shard  
* Attack Speed 0.7-1.3 → "**normal**" shard  
* Attack Speed \> 1.3 → "**heavy**" shard

#### **Damage Type**

Directly inherited from the weapon's damtype:

* **RED\_DAMAGE** → Red shards (Cardinal movement)  
* **WHITE\_DAMAGE** → White shards (Diagonal movement)  
* **BLACK\_DAMAGE** → Black shards (8-directional movement)  
* **PALE\_DAMAGE** → Pale shards (Teleport movement)

### **Usage Example**

1. Load a "kurokumo blade" (Average Requirement: 80, RED damage, Speed: 1.2).  
2. Activate disassembler.  
3. Receive 4-7 shards with:  
   * **Rarity 2** (80/30 \= 2.67 → 2\)  
   * **Normal** density (speed 1.2)  
   * **Red** damage type

These shards can then be used to move 6-10 units in cardinal directions on the crafting grid.


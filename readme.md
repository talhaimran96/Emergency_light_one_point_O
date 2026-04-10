## Presenting **Project Blackout: The Sustainable Backup**

### **The Motivation**
In the face of increasing **load shedding**, I wanted to build a reliable, high-quality light source that doesn't rely on the cheap lead-acid batteries found in most market units. Those units often fail within months and end up in a landfill. My goal was to create a repairable, modular light that can be maintained for years.

### **What It Does**
This is a compact emergency light powered by **two 18650 Lithium-ion cells**. It features a custom-designed **3D-printed housing** and modern **USB-C charging**. 

By using a dedicated **2S BMS**, the batteries are protected from overcharging and over-discharging, significantly extending their lifespan. The light source is a high-efficiency **3W COB LED** module, providing enough brightness for a standard room during an outage.

### **Sustainability & Cost-Efficiency**
While the initial assembly cost might be higher than a disposable light, the long-term economics are much better:
* **Modular Replacement:** When the batteries eventually degrade, you only need to swap the 18650 cells—not the whole device.
* **Repurposing Resources:** I found several listings on **Daraz** for "pulled" or pre-used 18650 cells. Using these high-quality salvaged batteries makes the project both cheaper and more eco-friendly.

---

### **System Architecture & Design**
The internal wiring ensures the 18650 cells are balanced and protected, while the exterior is designed for durability and ease of use.

#### **Circuit Diagram**
![Circuit Diagram](circuit%20diagram/Emergency%20light.png)

#### **Physical Build**
| Front View | Side View |
| :--- | :--- |
| ![Front View](picture/front.jpeg) | ![Side View](picture/side.jpeg) |

---

### **Parts List**
| Component | Quantity | Description |
| :--- | :---: | :--- |
| **COB LED Module** | 1 | 3W 3.7V 1000mA (300lm) |
| **18650 Batteries** | 2 | Lithium-ion cells (can be sourced as "pulled" cells) |
| **BMS Board** | 1 | 2S 8A Protection Board (Hx-2s-jh10) |
| **Charging Module** | 1 | 2S Type-C USB 18W Fast Charge with Temp Protection |
| **Buck Converter** | 1 | XL7015 DC-DC Step Down (to regulate voltage for the LED) |
| **Switch** | 1 | 2-Pin ON-OFF Toggle Switch |
| **Battery Holder** | 1 | 2x 18650 PCB Mount Holder |

---

### **3D Printing & Assembly**
The housing consists of two main parts designed for a snug fit and easy assembly. You can find the files in the `stl files/` directory:

* **`Emergencylight_body.stl`**: The main chassis that houses the batteries and electronics.
* **`Emergencylight_lid.stl`**: The top cover to secure the internals.

**Assembly Tips:**
1.  **Calibration:** If using pulled cells, ensure they are balanced before installing.
2.  **Voltage Regulation:** Use a multimeter to tune the XL7015 buck converter to the specific requirements of your COB LED.
3.  **Finish:** I recommend printing with 20% infill for a sturdy feel.


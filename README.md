# Automated 3D Printed Mini Disk Infiltrometer (AMDI)

The AMDI is a custom-designed, low-cost infiltrometer, primarily built using 3D printed parts. It features a Mariotte chamber, TDT sensor integration, and sintered stainless steel disk for accurate soil infiltration measurements.

---

## AMDI Overview

The following figure presents the fully assembled AMDI:

![AMDI](https://github.com/user-attachments/assets/d309d6c0-6ebe-4bdd-832e-cfcdc5c7396c)

---

## Parts and Slicer Settings

All parts except **A1 (infiltrometer body)** were printed using **Prusa XL**, **Prusa MK3S+**, and **Prusa Mini+** with settings provided in `!SlicerSettings.3mf`.

| Parameter                  | Value              |
|---------------------------|--------------------|
| Layer height              | 0.1 to 0.15 mm     |
| Extrusion multiplier      | 1.1                |
| Max print speed           | 15 mm/s            |
| Printing temperature      | 260 °C             |
| Wall thickness            | 2.5 mm             |
| Infill                    | 100%               |
| Cooler speed              | 15 to 20%          |
| Retraction length         | Disabled           |
| Infill/perimeters overlap | 20%                |

---

## Assembly of AMDI

### Required Components

- **O-rings**:
  - 1× 45 × 3.6 mm  
  - 1× 5 × 2.0 mm  
  - 3× 20 × 3.6 mm  

- **Other parts**:
  - 1× TMS-4 TDT sensor  
  - 1× Sintered stainless steel disk (Ø 45 mm, thickness 3 mm, 80 µm pore size, GKN GmbH, Germany)  
  - 3D printed parts:
    - Part A (A1 + A2)
    - Part B (B1 + B2)
    - Part C (lid)

---

### Assembly Instructions

1. **Bond the Printed Parts**  
   - Glue **B1 and B2** (Mariotte chamber and suction tube) using ethyl 2-cyanoacrylate (Henkel CEE GmbH, Germany). Let cure for **24 hours**.  
   - Repeat for:
     - **A1 and A2** (base + nozzle)
     - **C and the sintered disk**

2. **Install O-rings and Sensor**  
   - Insert **three 20 × 3.6 mm O-rings** into sensor openings.  
   - Apply a **non-silicone lubricant** (e.g., for plastic sewer pipes) to avoid damage.  
   - Carefully insert the **TMS-4 sensor**, with the **status diode facing the Mariotte chamber**.

3. **Assemble the Mariotte Chamber**  
   - The chamber (B1 + B2) has a **fixed suction tube** and **imprinted scale from 0 to −6 cm** in 0.5 cm increments.  
   - Connect the chamber to the Mariotte tube via **A2**, using a **5 × 2.0 mm O-ring**.  
   - Fill with water using a syringe **before mounting**.

4. **Slide the Chamber into Position**  
   - Use **sliders** on the chamber to mount it into the **rails of A1**, allowing adjustable height.

5. **Final Assembly**  
   - Fill the AMDI with **150 mL of water** (vs. 90 mL in conventional MDI).  
   - Screw on **Part C** with the **45 × 3.6 mm O-ring** and tighten to prevent leakage.

---

### Notes

- **Final dimensions**: 29.5 cm tall, 5 cm in diameter (22.5 cm without sensor).
- **Offset** between the Mariotte tube and sintered disk: **9 mm** — include this in **hydraulic conductivity (K)** calculations.
- The stainless-steel disk type is based on prior work by [Klípa et al., 2015] and [Zumr et al., 2019].

---

## Calibration and Measurement

_Section under construction..._

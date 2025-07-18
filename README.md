# Low-Cost Autonomous 3D-Printed Mini Disk Infiltrometer (AMDI)

## Introduction

The **Automated Mini Disk Infiltrometer (AMDI)** is a 3D-printed, low-cost device designed to measure **soil infiltration** under controlled suction conditions. Based on the principles of the widely used **Mini Disk Infiltrometer (MDI)**, the AMDI extends its functionality by integrating a **TMS-4 capacitance sensor** for automatic data collection, reducing the need for manual observation.

The AMDI is suitable for both **field** and **laboratory** use and enables the estimation of **unsaturated hydraulic conductivity** near saturation.

🚨 **Place order via email at jan-frantisek.kubat@fsv.cvut.cz or michal.snehota@cvut.cz. This offer is valid until withdrawn.**

---

## Future

To further establish the AMDI as a go-to instrument, the following steps are necessary to ensure a smooth user experience and maintain data integrity:

- Develop a software interface for calibration and measurement evaluation.
- Design a simpler calibration method that remains equivalent in accuracy but is more cost-effective.
- Conduct intensive field testing and implement modifications based on the collected data.
- Negotiate with TOMST company to integrate a native AMDI option into the TMS-4 software. 

---

## AMDI Overview

The following figure presents the fully assembled AMDI:

![AMDI](https://github.com/user-attachments/assets/d309d6c0-6ebe-4bdd-832e-cfcdc5c7396c)

---

## 3D Printing Overview

All 3D-printed parts were created using FDM printers such as **Prusa XL**, **MK3S+**, or **Mini+**. Recommended print settings are available in the provided `SlicerSettings.3mf` file.
AMDI was tested with polyethylene terephthalate glycol (PET-G) filament produced by Prusa a.s. (Czechia).
Use clear filament (color: E4E7E5) with a diameter of 1.75 ± 0.02 mm. Since the suction is set by adjusting the water level in the Mariotte chamber.

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

## Required Components

- **O-rings**:
  - 1× 45 × 3.6 mm  
  - 1× 5 × 2.0 mm  
  - 3× 20 × 3.6 mm  

- **Other parts**:
  - 1× TMS-4 TDT sensor [shop](https://tomst.com/web/en/systems/tms/tms-4/)
  - 1× Sintered stainless steel disk (Ø 45 mm, 3 mm thick)  
  - 3D printed parts:
    - A1 + A2 (infiltrometer body and base)
    - B1 + B2 (Mariotte chamber and suction tube)
    - C (lid)

---

## Assembly Instructions

1. **Bond Printed Parts**  
   - Glue A1 to A2, B1 to B2, and C to the disk using suitable adhesive.  
   - Allow to cure for 24 hours.

2. **Install O-rings and Sensor**  
   - Place O-rings into designated grooves.  
   - Lubricate before inserting the sensor to avoid damage.

3. **Assemble the Mariotte Chamber**  
   - Connect to the main body via O-ring seals.  
   - Use the integrated scale to adjust suction height.

4. **Final Assembly**  
   - Mount the chamber to the body rails using the sliders.  
   - Fill with water (approx. 150 mL), seal with the lid, and ensure no leakage.

> You can refer to the AI Assistant for help with assembly, calibration, and initial measurements: [AMDI AI-Assist](https://chatgpt.com/g/g-686f85880f7c81918232c61168e00342-amdi-ai-assistant).
> Assist is based on OpenAI ChatGPT.

---

## Calibration

Each AMDI device requires **individual calibration** to relate raw sensor signals to actual water volume. This ensures accurate measurement of infiltration.

General calibration steps:

1. Fill the reservoir and record weight loss over time on a precision balance.
2. Log the TMS-4 sensor signal simultaneously.
3. Fit the paired data using a polynomial regression (e.g., cubic).
4. Use only the active sensing region to avoid artifacts.

> Calibration details, procedures, and equations are available in the associated publication.

---

## Infiltration Measurements

The AMDI can be used under controlled or natural conditions to monitor infiltration at various pressure heads. The sensor enables automated data logging, making it suitable for both short-term and long-term infiltration studies.
Macro to calculate hydraulic conductivity: [Macro](https://library.metergroup.com/Sales%20and%20Support/METER%20Environment/New-Minidisk-Infiltrometer-Macro.xlsx?_gl=1*u4umky*_gcl_au*MTU2Mjk1ODM0OS4xNzUyMTM5NjQx)

> Refer to the associated article for detailed procedures and data analysis workflows.

---

## Modification

Modification is highly encouraged but must be credited. If feasible, please initiate a branch with the modification for review.

For example, it is not necessary for the Mariotte chamber (part B) to be detachable..

---

## Citation

If you use the AMDI in your work, please cite the related publication:

> [Author(s)], (2025). Title of the related article. *Journal Name*. DOI


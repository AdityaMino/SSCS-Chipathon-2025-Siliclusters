![IEEE SSCS](https://img.shields.io/badge/IEEE--SSCS-blue?style=for-the-badge&logo=ieee&logoColor=white)
![GF180MCU PDK](https://img.shields.io/badge/GF180MCU--PDK-orange?style=for-the-badge&logo=global-foundries)
![Open Source VLSI](https://img.shields.io/badge/Open--Source--VLSI-green?style=for-the-badge&logo=open-source-initiative&logoColor=white)

# 💡SSCS Chipathon 2025 Siliclusters
## ⚡Track: Digital Building Blocks

---

## 📝 About Project  
In our project, we are designing a **low-power, area-efficient 6T SRAM bitcell** optimized for the **GF180MCU-D  standard cell**.  
The goal is to develop a memory cell with enhanced **read stability, write margin, and leakage performance** for integration into open-source SoCs, supporting standard open-source tool flows.

We aim to make this a reusable, reliable memory building block for future **GF180MCU** projects by the community.

#### **PROJECT TRACKER - https://docs.google.com/spreadsheets/d/1I3WJNxxtnPEOm24B_O6vsVvTo-F7wX3jf2FrStrXF3M/edit?usp=sharing** 

---

## 📐 SRAM 6T Bitcell Specifications
### Process: GF180MCU-D
### Supply Voltage: 3.3 V (with target simulations down to 0.9 V)
### Drive Strength: Optimized for array integration
### Transistor Sizing: Balanced for read SNM, write margin, leakage

## 📊 Target PPA Metrics
| Metric            | Target         |
|-------------------|----------------|
| Area              | < 15 µm x 5 µm |
| Read SNM          | > 100 mV (target across corners) |
| Write Margin      | Robust at 0.9V |
| Standby Leakage   | Minimized via HV devices |
| Write Access Time | < 1 ns (preliminary goal) |

---

## 🔍 References  
- [Modica-SRAM](https://github.com/eda-ricercatore/Modica-SRAM)  
- [GF180MCU PDK Documentation](https://gf180mcu-pdk.readthedocs.io/en/latest/)  
- J. P. Kulkarni et al., “A 160mV Robust Schmitt Trigger Based Subthreshold SRAM,” IEEE JSSC, 2007  
- Pretl, H. et al., “Fifty nifty variations of two-transistor circuits,” IEEE SSC Magazine, 2021  

---

## 🎯 Objectives
1. Perform **schematic design** of the SRAM bitcell using Xschem with GF180MCU devices.
2. Run **read/write simulations** across PVT corners to optimize SNM and margins.
3. Develop **DRC/LVS-clean layout** using Magic with optimized area footprint.
4. Validate the layout through **netgen LVS** against schematic.
5. Perform **PEX extraction and SPICE simulations** for accurate behavior.
6. Create standard cell views for integration: **GDS, Verilog, Liberty, LEF**.

---

## 👥 Team Members
1. Aditya Minocha
2. Devansh Raut

---

## 📅 Timeline and Work Division

### Week 1 : 14 - 18 July  
**Task:** Schematic design, transistor sizing, and PVT simulations  
**Key Success:** Stable schematic achieving read/write functionality under 3.3V and 0.9V corners  

---

### Week 2 : 21 - 25 July  
**Task:** Initial layout in Magic following GF180MCU constraints  
**Key Success:** Clean DRC, compact layout for bitcell, preliminary array planning

---

### Week 3 : 28 July - 2 August  
**Task:** LVS validation, extraction, array assembly planning (2x2, 4x4)  
**Key Success:** LVS passed, matching schematic and layout netlists

---

### Week 4 : 2 August - 20 August  
**Task:** PEX simulations, detailed characterization (SNM, margins, leakage)  
**Key Success:** Clear simulation results, documented for comparison  

---

### Week 5 : 20 August - 5 September  
**Task:** Integration-ready views: Verilog, Liberty, LEF, GDS; documentation  
**Key Success:** Ready for array integration; results reproducible on GF180MCU tool flow  

---

## 📌 Notes

- This project uses **GF180MCU-D PDK (9T height)** for compatibility with existing OSU libraries.
- Simulation and characterization follow **open-source tools**: Xschem, Magic, Netgen, Ngspice.
- The final deliverable will contribute towards a potential **community open-source SRAM cell for GF180MCU**.

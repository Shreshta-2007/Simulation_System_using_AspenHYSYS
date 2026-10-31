# Simulation_System_using_AspenHYSYS
# Ethanol-Water Separation: Flash Separator and Distillation Column (Aspen HYSYS)

An Aspen HYSYS steady-state simulation of an ethanol-water separation process using a feed separator (V-100) and a distillation column (T-100), with a full report and hand calculations.

## Problem statement

Can a 50/50-ish ethanol-water feed be split into an ethanol-rich product and a water-rich product with one separator and one column?

This project simulates that in Aspen HYSYS using the NRTL model, which captures the non-ideal ethanol-water behaviour. A 100 kmol/h feed passes through a separator and a pump into a distillation column, which delivers 44.30 kmol/h of ethanol-rich distillate and 55.70 kmol/h of water-rich bottoms.

The report then goes beyond the software output: hand calculations check the material balance and compare the results with HYSYS, so the simulation isn't treated as a black box.

## Report

 [Aspen Hysys Project Report .pdf](https://github.com/user-attachments/files/34208512/Aspen.Hysys.Project.Report.pdf)
contains the simulation setup, results and hand calculations (material balance and [other checks]) compared against the HYSYS output.

## Process description

A 100 kmol/h ethanol-water feed at 25 °C and 101.3 kPa enters separator V-100. Only the liquid leaves the separator. Pump P-100 raises the pressure to 105 kPa, and the stream then goes to distillation column T-100, which splits it into an ethanol-rich distillate and a water-rich bottoms stream.

## Simulation setup

| Item | Setting |
|------|---------|
| Software | Aspen HYSYS V15 |
| Components | Ethanol, water |
| Property package | NRTL |
| Feed | 100 kmol/h (2924 kg/h), 25 °C, 101.3 kPa |
| Separator | V-100 |
| Pump | P-100, outlet 105 kPa |
| Column | T-100 [number of stages, feed stage, reflux ratio, specifications] |

## Key results

| Stream | Flow | Temperature |
|--------|------|-------------|
| Distillate (ethanol-rich) | 44.30 kmol/h | 78.27 °C |
| Bottoms (water-rich) | 55.70 kmol/h | 87.97 °C |

- Distillate ethanol purity: 79%
- Bottoms water purity: 21%
- Reflux ratio: 2.5
- Condenser and reboiler duties: 45 kmol/h

## Images
<img width="475" height="281" alt="Screenshot 2026-10-31 at 6 23 24 AM" src="https://github.com/user-attachments/assets/e3c70c84-722d-4d82-952c-9e8d507509fe" />
<img width="640" height="299" alt="Screenshot 2026-10-31 at 3 18 57 AM" src="https://github.com/user-attachments/assets/28766797-b536-4ff5-b590-fbeb419c42de" />
<img width="550" height="260" alt="Screenshot 2026-10-31 at 3 18 48 AM" src="https://github.com/user-attachments/assets/4bafa261-0f67-4a4e-b5fe-6a8341a1ec11" />


## Assumptions
- Steady state
- Ideal stages with the NRTL activity model for the ethanol-water non-ideality

## Similation could'nt be included as it is lincensed under college domain 

## Author

Shreshta Kanduri  | BITS Pilani Dubai B.E. Chemical Engineering  | www.linkedin.com/in/shreshta-kanduri-311230312

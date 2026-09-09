# Design and Implementation of a Microstrip Patch Antenna for 2.4 GHz ISM Band Applications

A CST Studio Suite-based microstrip patch antenna project designed for operation in the **2.4 GHz ISM band**. The project covers antenna geometry design, parametric/geometrical modification, electromagnetic simulation, fabrication, and experimental validation using a Vector Network Analyzer (VNA).

## Project Overview

The proposed antenna is a compact modified rectangular microstrip patch antenna designed on an **FR-4 substrate**. The structure uses an inset-fed microstrip line and additional slots/notches to improve impedance matching and resonant behavior.

According to the accompanying lab report, the substrate dimensions are **60 mm × 60 mm × 1.6 mm**, with a dielectric constant of **4.3**. The optimized simulated design resonates at approximately **2.41 GHz** with a minimum simulated S11 of **−18.64 dB** and a realized gain of approximately **1.86 dBi**.

## Objectives

- Design a compact microstrip patch antenna for the 2.4 GHz ISM band.
- Investigate the effect of geometrical variations on antenna performance.
- Optimize the antenna dimensions for improved impedance matching and radiation characteristics.
- Evaluate S11, gain, efficiency, VSWR, and radiation patterns.
- Fabricate the proposed antenna and experimentally validate it using a VNA.

## Antenna Design

The antenna consists of:

- Rectangular radiating patch
- Inset-fed microstrip feed line
- FR-4 dielectric substrate
- Ground plane on the opposite side
- Two rectangular top notches
- Feed-side slots

The feed line was designed for approximately **50 Ω** input impedance.

## Final Geometrical Parameters

| Parameter | Description | Value |
|---|---|---:|
| SL | Substrate Length | 60 mm |
| SW | Substrate Width | 60 mm |
| PL | Patch Length | 28 mm |
| PW | Patch Width | 31.5 mm |
| FW | Feed Line Width | 3.1 mm |
| NSW | Top Notch Width | 4 mm |
| NSL | Top Notch Depth | 6.1 mm |
| ST | Feed Side Slot Width | 4.58 mm |
| SLOT_L | Feed Side Slot Depth | 7 mm |
| SH | Substrate Thickness | 1.6 mm |
| GH | Copper Thickness | 0.035 mm |

## Design Evolution

The report presents three antenna configurations:

1. **Antenna 1:** Basic rectangular patch.
2. **Antenna 2:** Modified patch geometry for improved impedance matching.
3. **Antenna 3:** Additional slots and notches, producing improved return-loss characteristics and resonance near the target ISM band.

## Simulation Results

The final simulated antenna achieved:

| Parameter | Simulated Result |
|---|---:|
| Resonant Frequency | 2.41 GHz |
| Minimum S11 | −18.64 dB |
| Reflection Coefficient | 0.1168 |
| VSWR | 1.26 |
| Realized Gain | ≈ 1.86 dBi |

The simulated S11 is below −10 dB around the resonant frequency, indicating good impedance matching.

## Radiation Characteristics

The simulated H-plane and E-plane radiation patterns at 2.4 GHz show a clear main lobe and stable radiation characteristics. The results indicate that the antenna is suitable for short-range wireless communication applications in the ISM band.

## Fabrication and Measurement

The antenna was fabricated on an FR-4 substrate and experimentally characterized using a **Vector Network Analyzer (VNA)**.

The measured response reported in the accompanying document shows:

| Parameter | Simulated | Measured |
|---|---:|---:|
| Resonant Frequency | 2.41 GHz | 3.18 GHz |
| Return Loss (S11) | −18.64 dB | −29.96 dB |
| Reflection Coefficient | 0.1168 | 0.0318 |
| VSWR | 1.26 | 1.07 |

A noticeable frequency shift occurs between simulation and measurement. The report attributes the difference to practical factors including FR-4 material variation, fabrication tolerances, substrate-thickness variation, SMA connector and soldering effects, measurement uncertainties, conductor/material losses, feed imperfections, and idealized simulation assumptions.

## CST Model

The repository contains the CST model and the original CST project archive:

```text
CST_Model/
├── CST_SAFIT.cst
└── CST_SAFIT_2_ProjectArchive.zip
```

Open `CST_SAFIT.cst` using a compatible version of **CST Studio Suite**. The project archive is included as an additional backup/reference copy.

## Figures

Selected figures extracted from the report are included for quick reference:

```text
Figures/
├── antenna_geometry.png
├── geometrical_dimensions.png
├── simulated_s11.png
├── efficiency_gain_vswr.png
├── radiation_patterns.png
├── fabrication_vna_setup.png
└── simulated_measured_comparison.png
```

## Documentation

The complete lab report is included here:

```text
Documentation/microwave_engineering_lab_report.pdf
```

The report covers the antenna design, geometrical dimensions, design evolution, simulated results, fabrication, experimental results, simulated-versus-measured comparison, engineering-problem discussion, conclusion, and references.

## Software

- CST Studio Suite
- Vector Network Analyzer (for experimental validation)

## Applications

The proposed antenna is intended for short-range wireless communication applications in the 2.4 GHz ISM band, including potential Wi-Fi, IoT, and wireless sensor-network applications.

## Repository Structure

```text
iot-microstrip-patch-antenna-2.4ghz/
│
├── CST_Model/
│   ├── CST_SAFIT.cst
│   └── CST_SAFIT_2_ProjectArchive.zip
│
├── Figures/
│   ├── antenna_geometry.png
│   ├── geometrical_dimensions.png
│   ├── simulated_s11.png
│   ├── efficiency_gain_vswr.png
│   ├── radiation_patterns.png
│   ├── fabrication_vna_setup.png
│   └── simulated_measured_comparison.png
│
├── Documentation/
│   └── microwave_engineering_lab_report.pdf
│
└── README.md
```

## Author

**Shahziar Karim Safit**  
Department of Electrical & Electronic Engineering  
Rajshahi University of Engineering & Technology (RUET)

## Team Members

- Ankon Datta
- Shahziar Karim Safit
- Md. Jubayer Hossain Shawon

## References

The complete references used in the accompanying report are available in `Documentation/microwave_engineering_lab_report.pdf`.

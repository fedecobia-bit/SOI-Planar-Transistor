# SOI pMOS FD-SOI – Integrated Systems Technology, Final Project

**Authors:** Davide Cameran, Lucas F. V. Cançado, Federico Cobianchi, Simone Telesca

## Objective

Design, simulate with Sentaurus TCAD, and electrically characterise a pMOS transistor on an SOI wafer with a nominal channel length of 80 nm.

The project followed this path:

1. Planar pMOS design, equivalent to the nMOS used in the first laboratory experience (Appendix A).
2. Move to a pMOS SOI FD (Fully Depleted) with standard SOI layers (Si 60 nm, BOX 190 nm).
3. Final move to a pMOS UTTB FD-SOI (Ultra-Thin Body and BOX), with Si ≈ 25 nm and BOX ≈ 50 nm, to improve DIBL. In the standard SOI version DIBL was about twice the ideal value (~60 mV/V), measured at 111 mV/V.

## Report structure

The report (`Group17_CameranCancadoCobianchiTelesca_ReportPROJECT.pdf`) is organised as follows:

- **Ch. 1 – Introduction:** technological parameters (doses, energies, implant angles) and structure dimensions.
- **Ch. 2 – Pen & paper design:** preliminary estimates of doses, energies, minimum gate oxide thickness, and theoretical threshold voltage.
- **Ch. 3 – Fabrication:** process steps with simulated intermediate results:
  - 3.1 Substrate definition (p-type, Boron 1·10¹⁵ cm⁻²).
  - 3.2 Gate creation (double Arsenic implant for the n-well, dry oxidation at 850 °C for 10 min, polysilicon deposition and etching).
  - 3.3 LDD (Boron, 4 keV, 4·10¹⁴ cm⁻²), preceded by a protective oxidation of the gate.
  - 3.4 Spacers in Si₃N₄ via deposition and anisotropic etching.
  - 3.5 HDD (BF₂, 10 keV, 4.5·10¹⁵ cm⁻², 7° tilt) with RTA at 950 °C.
  - 3.6 Aluminium contacts (source/drain and gate, using two photoresists).
  - 3.7 Complete structure, mirrored about the vertical axis.
- **Ch. 4 – Electrical characterisation:** I-V simulation (V_DS = 1 V and 0.1 V, V_GS = –1 V) and FOM extraction.
- **Ch. 5 – Conclusion.**
- **Appendix A – Planar pMOS:** full process sequence and I-V characteristics of the starting device.

## Main results (UTTB pMOS FD-SOI)

| Parameter | Value |
|---|---|
| I_ON | 8.54 · 10⁻⁵ A |
| I_OFF | 1.15 · 10⁻¹¹ A |
| I_ON / I_OFF | ≈ 7.4 · 10⁶ |
| V_th \|V_DS=1V | –0.62 ± 0.01 V |
| V_th \|V_DS=0.1V | –0.68 ± 0.01 V |
| SS | 101 mV/dec |
| DIBL | 66.7 ± 15.7 mV/V |

DIBL was reduced compared with the standard SOI version (111 mV/V), but it remains above the ideal value of about 60 mV/V.

## References

The full bibliography is in the report (section "Bibliography"), including: Verma & Abdullah (2015), Mahmoud et al. (2019), Honan (RIT), Cho et al. (1985), Lacord et al. (SISPAD 2023), and Aziz et al. (ARPN JEAS, 2016). Figures 3.2, 3.4 and 3.5 come from the *Physics of Technological Processes* course notes (Prof. M. Cocuzza) and from Wolf & Tauber, *Silicon Processing for the VLSI Era*, Vol. 1.

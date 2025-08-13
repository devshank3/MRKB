## Introduction 

Image optimizations and suggested protocols, most frequently used Pulse sequences 


Manufacturer acronyms comparison:

| Pulse Sequence/Imaging        | GE           | Philips      | Siemens      | Option         |
|-------------------------------|--------------|--------------|--------------|----------------|
| Spin echo                     | Spin echo    | Spin echo    | Spin echo    |                |
| Fast spin echo                | FSE          | TSE          | TSE          |                |
| Coherent gradient echo        | GRASS        | FFE          | FISP         |                |
| Balanced gradient echo        | FIESTA       | BFFE         | True FISP    |                |
| Incoherent gradient echo      | SPGR         | T1 FFE       | FLASH        |                |
| Steady state free precession  | SSFP         | T2 FFE       | PSIF         |                |
| Inversion recovery (IR)       | IR           | IR           | IR           |                |
| Short TI inversion recovery   | STIR         | STIR         | STIR         |                |
| Fluid attenuated inversion recovery   | FLAIR        | FLAIR        | FLAIR        |                |
| Presaturation                 | SAT          | REST         | SAT          |                |
| Gradient moment nulling       | FC           | FC           | GMR          |                |
| Respiratory compensation      | RC           | PEAR         | RC           |                |
| Signal averaging              | NEX          | NSA          | AC           |                |
| Partial averaging             | Fractional NEX| Half scan   | Half Fourier |                |
| Oversampling                  | No phase wrap| Fold over suppression   | Oversampling |                |
| Rectangular/asymmetric        | Rectangular  | Rectangular  | Undersampling|                |
| FOV                           | FOV          |              |              |                |

---

### Spin echo (SE) 

Also known as Conventional Spin Echo (CSE). 

Uses a 90° excitation pulse followed by a 180° rephasing pulse to produce a spin echo.
Sometimes variable flip angle could also be used. 

SE pulse sequences are the most commonly implemented sequences as they produce optimum SNR and CNR.

For T1 weighting one SE is used: 
- short TE min–20 ms 
- short TR 300–600 ms 

For PD/T2 weighting 2 SE's are used:
- short TE 20 ms (first echo PD)
- long TE 70 ms (second echo T2)
- long TR 2000 ms

---

### Fast Spin echo (FSE) or TSE - Turbo spin echo 

Fast spin echo (FSE) uses a 90° flip angle followed by several 180° rephasing
pulses to produce several spin echoes in a given TR.

Data from each echo are collected and stored in a different line of K space.
FSE can be used to produce either one or two echoes as in SE.



---

### Inversion recovery (IR/IR-FSE)

---

### Coherent gradient echo (GRE) (T2*)

---

### Balanced gradient echo (GRE) (T2*)

---


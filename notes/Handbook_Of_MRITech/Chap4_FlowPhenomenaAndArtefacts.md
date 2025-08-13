## Introduction

Flow phenomena remedies and Artefact problems to be considered under Image optimization

Types of flow phenomena:

1. Time of flight (TOF)
2. Entry slice phenomena 
3. Intra-Voxel dephasing


### Time of flight (TOF)

Time of flight phenomenon occurs when moving nuclei (like flowing blood) don't receive the complete RF pulse sequence needed for proper signal generation.

**Mechanism:**
- **GRE sequences**: More tolerant - gradient rephasing is not slice selective, so nuclei can produce signal if excited at any point
- **SE sequences**: Problematic - require both 90° excitation and 180° rephasing pulses in same slice
  - Signal loss occurs when nuclei exit slice between pulses
  - Can cause signal enhancement or loss from flowing nuclei

**Clinical solution:** Presaturation pulses placed upstream from imaging FOV to saturate flowing spins before they enter

---

### Entry slice phenomena

---

### Intra-Voxel dephasing 

---

## Artefacts 

Common types of artefacts are 

- Phase mismapping (motion)
- Aliasing (wrap)
- Chemical shift
- Chemical misregistration
- Truncation
- Magnetic susceptibility.
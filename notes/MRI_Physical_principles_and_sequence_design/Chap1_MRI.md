
### 1.1 Magnetic Resonance Imaging: The Name

Magnetic Resonance Imaging (MRI) is a discipline in applied sciences of NMR. 
It's mainly used for imaging soft tissues in the human body and metabolic processes, thus having a strong position in biomedical science applications.

MRI is a powerful imaging modality due to its flexibility and sensitivity to a broad range of tissue properties. 

One of the main advantages of MRI is its relative safety and non-invasive nature.

MRI stems from the application of nuclear magnetic resonance (NMR) to radiological imaging. 

The term 'magnetic' refers to the use of various magnetic fields, and 'resonance' refers to the need to match the frequency of an oscillating magnetic field to the precessional frequency of a nucleus's spin in a tissue molecule. The term 'nuclear' in this context refers to the benign role of the nucleus's spin in the process, not to anything harmful or dangerous. 

The term 'nuclear' has been largely avoided due to public concern, leading to the widespread use of the acronym 'MRI' instead of 'NMRI'.

---

### 1.2 The Origin of Magnetic Resonance Imaging

- The origins of MRI can be traced back to 1973 with significant contributions from Lauterbur and Mansfield.

- The concept of MRI is based on the known fact that the spin of a hydrogen nucleus (proton) in a magnetic field precesses around the field at the 'Larmor frequency', which depends linearly on the field's magnitude.

- Lauterbur and Mansfield proposed that if a spatially varying magnetic field is applied to an object, the Larmor frequencies will also vary spatially.
- By separating different frequency components of the signal, they could obtain spatial information about the object. This concept of spatially encoding the data was crucial for MR imaging.

- The principle of using a magnetic field gradient to capture the essence of MRI was a breakthrough idea.

- The concept of nuclear magnetic resonance is rooted in the discovery of the proton's spin.

    In the 1930s, Rabi and coworkers studied the spin of the proton and its interaction with a magnetic field, building on the earlier work of Stern and Gerlach.
    In 1946, Bloch and Purcell extended these early quantum mechanical concepts to measure the precession effect of the spins around a magnetic field. 
    
    They successfully measured a precessional signal from a water sample and a paraffin sample and explained many experimental and theoretical details still in use today.

    Bloch and Purcell were awarded the Nobel prize in physics in 1952 for their work.

---

### 1.3 Overview of MRI Concepts

#### 1.3.1 Fundamental Interaction of a Proton Spin with the Magnetic Field

- MRI relies on the interaction of nuclear spins, primarily hydrogen protons, with an external magnetic field.
- This interaction causes proton spins to precess around the direction of the external magnetic field, represented as \( \vec{B}_0 \).
- Proton spins can be visualized as electrically charged spinning gyroscopes, forming an effective current loop that interacts with magnetic fields.
- The magnetic dipole moment vector \( \vec{\mu} \) describes the strength of this interaction and aligns with the external magnetic field, similar to a compass needle.
- Instead of aligning directly with the field, the magnetic moment vector precesses around the field direction due to its spin, akin to gyroscopic motion.
- The precession angular frequency, known as the Larmor frequency, is determined by the Larmor equation: \( \omega_0 = \gamma B_0 \).
- The gyromagnetic ratio \( \gamma \) for hydrogen protons in water is approximately \( 2.68 \times 10^8 \) rad/s/tesla.
- For a magnetic field strength of 2 Tesla, the precession frequency is 85.2 MHz, just below the FM radio frequency range.

Precession 

By definition, precession is the circular motion of the axis of rotation of a spinning body about another fixed axis caused by the application of a torque in the direction of the precession.

https://en.wikipedia.org/wiki/Precession

<p align="center">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/82/Gyroscope_precession.gif/220px-Gyroscope_precession.gif" alt="Precession Diagram" width="200">
</p>
<p align="center">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/bb/Praezession.svg/800px-Praezession.svg.png" alt="Precession Diagram" width="200">
</p>

---

#### 1.3.2 Equilibrium Alignment of Spin

- Proton magnetic moments do not fully align with the external magnetic field due to thermal energy at body temperature.
- Thermal energy is much larger than the quantum energy difference between parallel and anti-parallel spin alignments.
- Protons have two quantum spin states with corresponding energy levels; the Larmor precession frequency is related to this energy difference.
- The smallness of quantum spin energy relative to thermal energy results in a minimal 'spin excess' (more spins parallel than anti-parallel to the field).
- The spin excess is quantified by the formula: \( \text{spin excess} \approx N \frac{\bar{h}\omega_0}{2kT} \), where \( N \) is the total number of spins.
- Despite the small spin excess, a significant signal can still be detected due to the large number of protons in tissue.
- The longitudinal equilibrium magnetization \( M_0 \) is the average magnetic dipole density along the field direction.
- \( M_0 \) is calculated using the formula \( M_0 = \rho_0 \frac{\gamma^2 \bar{h}^2}{4kT} B_0 \), where \( \rho_0 \) is the proton spin density.

---

#### 1.3.3 Detecting the Magnetization of the System

- For a detectable MRI signal, the magnetization vector must be tipped away from the external magnetic field direction to initiate precession.
- This is achieved by applying a radiofrequency (rf) pulse, which rotates the magnetization vector into the transverse plane, creating transverse magnetization.
- The rf pulse is tuned to the Larmor frequency to ensure resonance and synchronize the precessing spin.
- A \( \pi/2 \)-pulse rotates longitudinal magnetization into the x-y plane, leading to transverse magnetization that precesses with a sinusoidal time dependence.
- The complex magnetization is expressed as \( M_+(t) = M_x(t) + iM_y(t) = M_0 e^{-i\omega_0 t + i\phi_0} \), where \( \phi_0 \) is the initial phase angle.
- The induced signal in the receive coil results from the rotating transverse magnetization, described by the electromotive force (emf).
- The emf is calculated as \( \text{emf} = -\frac{d}{dt} \int d^3r \, \vec{M}(\vec{r}, t) \cdot \vec{B}_{\text{receive}}(\vec{r}) \), and is proportional to the Larmor frequency \( \omega_0 \) and the magnetization \( M_0 \).
- The MRI signal depends on the square of the static magnetic field, as shown by \( \text{signal} \propto \gamma^3 B_0^2 \rho_0 T \).
- Increasing the magnetic field strength improves the signal, which is a key factor in optimizing MRI performance.

---

#### 1.3.4 Magnetic Resonance Spectroscopy

- Hydrogen protons in different molecules experience slightly different magnetic environments, causing variations in the local Larmor frequency, known as chemical shifts.

- Chemical shift imaging adds a frequency dimension to MRI, allowing differentiation between molecular species based on their local magnetic fields.

- Each species contributes uniquely to the total MRI signal due to its specific Larmor frequency.

- The signal expression for transverse magnetization incorporates contributions from various species: (\text{signal} \propto \sum_j M_0(j) \omega_0(j) e^{-i\omega_0(j)t + i\phi_0(j)}).

- Magnetic resonance spectroscopy aims to determine the relative amplitudes of different frequency components to identify spin densities of different molecular species.

- A Fourier transform is used to convert the time-domain signal into a frequency domain, aiding in the analysis of chemical shifts.

- Chemical shift imaging helps spatially separate signals from different tissue components, such as distinguishing between water and fat.

---

#### 1.3.5 Magnetic Resonance Imaging

- MRI aims to link signal measurements with spatial locations of proton sources.  
- In a uniform magnetic field, the total signal reflects all protons of a single chemical species, like water.  
- Adding a spatially varying magnetic field introduces spatially varying frequency components: \(\omega(x) = \gamma B(x)\).  
- These frequency components provide spatial information, enabling signal inversion and object reconstruction.  
- Fourier transforms facilitate the transition between signal space and image space, allowing for 2D and 3D imaging.  
- A linear gradient coil modifies the magnetic field linearly, enabling spatial encoding of signals.  
- An rf excitation pulse with a finite bandwidth targets a specific slice of spins orthogonal to the gradient.  
- Gradient coil configurations allow for flexible slice orientations without physically rotating the sample.  
- The central frequency and bandwidth of the rf pulse determine the slice thickness and offset from the origin.

---

#### 1.3.6 Relaxation Times

- Relaxation times affect the MRI signal strength, involving interactions of spins with their environment.  
- **T1 (Longitudinal Relaxation Time):**   
  - Describes the regrowth of magnetization along the static field direction after being tipped into the transverse plane.  
  - Characterized by \[ M_z(t) = M_0(1 - e^{-t/T1}) \].  
  - Affects signal suppression if data is sampled before full regrowth.  
   
- **T2 (Transverse Relaxation Time):**  
  - Represents spin-spin decay, leading to dephasing of transverse magnetization.  
  - Given by \[ M_\perp(TE) = M_0(1 - e^{-TR/T1})e^{-TE/T2} \].  
  - Causes coherence loss between spins due to local frequency variations.  
   
- **T2 (Effective Transverse Relaxation Time):**  
  - Accounts for additional dephasing from external field inhomogeneities.  
  - Rephasing techniques, like 180° pulse, can counteract this dispersion.  
   
---

#### 1.3.7 Resolution and Contrast

- These relaxation parameters (spin density, T1, T2) are crucial for MRI and are explored in detail in subsequent chapters.

- MRI resolution is independent of the rf field wavelength, achieving millimeter-scale resolution.  
- Resolution is influenced by signal and noise sampling, filtering, proton diffusion, and magnetic field nonuniformities.  
- MRI's versatility stems from its sensitivity to various factors like proton densities, relaxation times, temperature, proton motion, chemical shifts, and tissue heterogeneity.  
- Different contrast levels can be generated based on these variables, enhancing MRI's utility compared to single-contrast imaging techniques.  
- **Contrast Mechanisms:**  
  - For long TR and short TE, images are sensitive to tissue spin density.  
  - For TE ≈ T2 and long TR, images are weighted by both spin density and T2, enhancing contrast between tissues with different T2.  
  - For TR ≤ T1 and short TE, images are weighted by both spin density and T1.  
- These factors allow MRI to produce diverse and detailed imaging contrasts.

---

#### 1.3.8 Magnetic Field Strength

- Higher magnetic field strengths improve the signal-to-noise ratio (SNR) in MRI.  
- Low-field machines (<0.5 T) are cheaper but have lower SNR compared to mid (0.5-1.0 T) and high-field (>1.0 T) machines.  
- The MRI signal increases quadratically with field strength, while noise increases linearly at high fields.  
- Experimental validation shows linear SNR growth with field strength from 0.5 T to 7.0 T.  
- Concerns with higher fields include rf heating and nonuniform rf fields.  
- At 1.0 T, the rf frequency is 42.6 MHz, with a seven-meter free-space wavelength.  
- Higher fields reduce rf wavelengths below 1m only above 7.0 T.  
- In vivo, the relative permittivity reduces the effective wavelength to about 1m at 1T.  
- Rf pulse and coil design considerations are crucial at higher field strengths.

#### 1.3.9 Key Developments in Magnetic Resonance

- **Echoing Mechanisms:**  
  - Spin echo and gradient echoes help recover signals lost to transverse relaxation.  
  - Spin echo uses multiple rf pulses to address inhomogeneous magnetic fields, crucial for T2-weighted imaging.  
   
- **Artifacts Leading to Innovations:**  
  - MR angiography emerged from efforts to eliminate flow and motion blurring, enhancing blood vessel imaging.  
  - Functional MRI (fMRI) developed from observing signal changes due to magnetic susceptibility differences, allowing detection of brain activity.  
   
- **Improvements in Imaging Speed:**  
  - Original spin echo scans were slow; fast gradient echo methods reduced scan times significantly.  
  - Echo planar methods enabled rapid data acquisition with gradient echoes.  
  - Parallel imaging uses multiple rf coils to further speed up imaging.  
   
- **Challenges and Solutions:**  
  - Magnetic field inhomogeneities can cause image distortion.  
  - Improved magnet design and sequence designs are addressing these issues.  
   
- These developments enhance MR angiography, brain imaging, and cardiac MRI, with detailed discussions in later chapters.
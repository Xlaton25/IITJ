# PART 1: Structure-Processing-Property Relationships, Mechanical Testing & Theories of Failure

**Course:** Materials Design and Evaluation Techniques (MEL7250 / MEL7100)  
**Instructor Style:** Prof. Rahul Chhibber (IIT Jodhpur)  
**Coverage:** Module 1 & Module 2

---

## TABLE OF CONTENTS

1. [Module 1.1: Classification of Materials & Crystal Structures](#1-classification-of-materials--crystal-structures)
2. [Module 1.2: Phase Diagrams, Solidification & Nucleation](#2-phase-diagrams-solidification--nucleation)
3. [Module 1.3: Tensile Testing, Stress-Strain Relations & Plastic Instability](#3-tensile-testing-stress-strain-relations--plastic-instability)
4. [Module 1.4: Compression, Hardness & Impact Testing](#4-compression-hardness--impact-testing)
5. [Module 1.5: Fatigue & Creep Behavior](#5-fatigue--creep-behavior)
6. [Module 2: Theories of Failure & Multiaxial Stress Analysis](#6-theories-of-failure--multiaxial-stress-analysis)
7. [Professor's High-Frequency Exam Question Bank (Solvers & Pitfalls)](#7-professors-high-frequency-exam-question-bank)

---

# 1. Classification of Materials & Crystal Structures

### 1.1 Classes of Engineering Materials

- **Metals & Alloys:** Characterized by non-directional metallic bonding, delocalized electron cloud, high electrical/thermal conductivity, ductility, and lustrous appearance.
- **Ceramics:** Covalent and ionic bonding, high hardness, high compressive strength, high melting temperatures, chemical inertness, but inherently brittle with low fracture toughness ($K_{1c} \sim 1 - 5\text{ MPa}\sqrt{\text{m}}$).
- **Polymers:** Covalently bonded macromolecular carbon chains held by secondary Van der Waals forces; low density, low stiffness, viscoelastic, and temperature-sensitive.
- **Composites:** Synergistic combinations of matrix (polymer, metal, ceramic) and reinforcement (fibers, whiskers, particles) engineered for high specific strength ($\sigma/\rho$) and specific modulus ($E/\rho$).

### 1.2 Crystal Geometry & Atomic Diameter Formulations

For cubic systems with lattice parameter $a$:

- **Body-Centered Cubic (BCC) (e.g., $\alpha$-Fe, W, Mo, Cr):**
  - Coordination Number: $8$; Atoms per unit cell: $N = 2$.
  - Close-packed direction: Body diagonal $\rightarrow 4r = a\sqrt{3}$.
  - Atomic Radius: $r = \frac{a\sqrt{3}}{4}$.
  - **Atomic Diameter:**
    $$d = 2r = \frac{a\sqrt{3}}{2} \quad \text{or} \quad \frac{a}{4/\sqrt{3}}$$
- **Face-Centered Cubic (FCC) (e.g., $\gamma$-Fe, Al, Cu, Ni):**
  - Coordination Number: $12$; Atoms per unit cell: $N = 4$.
  - Close-packed direction: Face diagonal $\rightarrow 4r = a\sqrt{2}$.
  - Atomic Radius: $r = \frac{a\sqrt{2}}{4} = \frac{a}{2\sqrt{2}}$.
  - **Atomic Diameter:**
    $$d = 2r = \frac{a\sqrt{2}}{2} = \frac{a}{\sqrt{2}}$$

---

# 2. Phase Diagrams, Solidification & Nucleation

### 2.1 The Iron-Iron Carbide ($\text{Fe-Fe}_3\text{C}$) Phase Diagram

- **Key Invariant Reactions:**
  - **Eutectic ($1147^\circ\text{C}$):** $L(4.3\%\text{ C}) \rightleftharpoons \gamma(2.14\%\text{ C}) + \text{Fe}_3\text{C}(6.67\%\text{ C})$ [Ledeburite]
  - **Eutectoid ($727^\circ\text{C}$):** $\gamma(0.77\%\text{ C}) \rightleftharpoons \alpha(0.022\%\text{ C}) + \text{Fe}_3\text{C}(6.67\%\text{ C})$ [Pearlite]
- **Phase Fractions via Lever Rule:**
  For an alloy of composition $C_0$ at temperature just below $727^\circ\text{C}$:
  - Total Cementite ($\text{Fe}_3\text{C}$):
    $$W_{\text{Fe}_3\text{C}} = \frac{C_0 - 0.022}{6.67 - 0.022}$$
  - Total Ferrite ($\alpha$):
    $$W_\alpha = \frac{6.67 - C_0}{6.67 - 0.022}$$
  - For **Hypoeutectoid Steel** ($C_0 < 0.77\%\text{ C}$):
    $$W_{\alpha,\text{pro}} = \frac{0.77 - C_0}{0.77 - 0.022}, \quad W_{\text{pearlite}} = \frac{C_0 - 0.022}{0.77 - 0.022}$$
  - For **Hypereutectoid Steel** ($0.77\% < C_0 < 2.14\%\text{ C}$):
    $$W_{\text{Fe}_3\text{C},\text{pro}} = \frac{C_0 - 0.77}{6.67 - 0.77}, \quad W_{\text{pearlite}} = \frac{6.67 - C_0}{6.67 - 0.77}$$

### 2.2 Thermodynamics of Solidification & Nucleation

- **Homogeneous Nucleation:**
  The total free energy change $\Delta G$ for a spherical solid nucleus of radius $r$ formed in supercooled liquid is:
  $$\Delta G = \frac{4}{3}\pi r^3 \Delta G_v + 4\pi r^2 \gamma$$
  Where:
  - $\Delta G_v = -\frac{\Delta H_f \Delta T}{T_m}$ is the volume free energy driving force ($\Delta H_f$ = latent heat of fusion, $\Delta T = T_m - T$ = degree of supercooling).
  - $\gamma$ is the solid-liquid interfacial energy ($J/\text{m}^2$).
  - **Critical Radius ($r^*$):** Setting $\frac{d(\Delta G)}{dr} = 0$:
    $$r^* = -\frac{2\gamma}{\Delta G_v} = \frac{2\gamma T_m}{\Delta H_f \Delta T}$$
  - **Activation Free Energy Barrier ($\Delta G^*$):**
    $$\Delta G^* = \frac{16 \pi \gamma^3}{3 (\Delta G_v)^2} = \frac{16 \pi \gamma^3 T_m^2}{3 (\Delta H_f)^2 (\Delta T)^2}$$
- **Heterogeneous Nucleation:**
  Occurs on foreign mold walls or nucleating agents with contact angle $\theta$:
  $$\Delta G^*_{\text{het}} = \Delta G^*_{\text{hom}} \cdot S(\theta)$$
  Where the shape factor $S(\theta)$ is:
  $$S(\theta) = \frac{(2 + \cos\theta)(1 - \cos\theta)^2}{4}$$
  _(For $\theta = 90^\circ$: $\cos 90^\circ = 0 \implies S(90^\circ) = \frac{2 \times 1}{4} = 0.5 \implies \Delta G^__{\text{het}} = \frac{1}{2}\Delta G^\*_{\text{hom}}$)\*.

---

# 3. Tensile Testing, Stress-Strain Relations & Plastic Instability

### 3.1 Engineering vs. True Parameters

| Parameter  | Engineering                                      | True                                                                      | Mathematical Interrelation                                                   |
| :--------- | :----------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------- |
| **Stress** | $s = \frac{P}{A_0}$                              | $\sigma = \frac{P}{A}$                                                    | $\sigma = s(1 + e) = s \cdot e^\varepsilon$ (prior to necking)               |
| **Strain** | $e = \frac{\Delta L}{L_0} = \frac{L - L_0}{L_0}$ | $\varepsilon = \int_{L_0}^L \frac{dL}{L} = \ln\left(\frac{L}{L_0}\right)$ | $\varepsilon = \ln(1 + e) = \ln\left(\frac{A_0}{A}\right)$ (constant volume) |

- **Additivity of True Strain:** True strains are additive: $\varepsilon_{\text{total}} = \varepsilon_1 + \varepsilon_2 + \dots$ (whereas engineering strains are not).

### 3.2 Considère's Criterion for Tensile Instability (Necking)

Necking begins at the maximum load ($P_{\max}$), where $dP = 0$:
$$P = \sigma A \implies dP = \sigma dA + A d\sigma = 0 \implies \frac{d\sigma}{\sigma} = -\frac{dA}{A} = d\varepsilon$$
$$\mathbf{\frac{d\sigma}{d\varepsilon} = \sigma}$$

- For a material following Hollomon’s power-hardening law ($\sigma = K \varepsilon^n$):
  $$\frac{d\sigma}{d\varepsilon} = n K \varepsilon^{n-1} = \frac{n \sigma}{\varepsilon}$$
  Setting $\frac{n\sigma}{\varepsilon} = \sigma \implies \mathbf{\varepsilon_u = n}$
- The true uniform strain at the onset of necking is numerically equal to the work-hardening exponent $n$.
- Ultimate Tensile Strength in terms of $K$ and $n$:
  $$s_u = \text{UTS} = K n^n e^{-n}$$

### 3.3 Tensile Behavior of Brittle Materials (Ceramics)

- In silica, alumina, and glasses, plastic deformation is negligible ($\varepsilon_p \approx 0$).
- Fracture takes place abruptly at maximum load without necking.
- Fracture strain: $\varepsilon_f = \ln(L_f / L_0) = \ln(A_0 / A_f)$.

---

# 4. Compression, Hardness & Impact Testing

### 4.1 Compression Testing & Barreling

- **Frictional Restraint:** Friction between the cross-head platens and test specimen restricts radial lateral expansion at the ends.
- **Barreling:** The unrestrained midsection bulges outwards, creating a non-uniform triaxial stress state.
- **Flow Curve Concavity:** Friction and barreling falsely increase the required compressive load, causing an artificial upward curvature (concavity) in the compressive stress-strain curve.

### 4.2 Hardness Testing

- **Brinell Hardness Test (BHN):** Hardened steel or tungsten carbide ball of diameter $D$ applied under load $P$:
  $$\text{BHN} = \frac{2P}{\pi D \left(D - \sqrt{D^2 - d^2}\right)}$$
- **Vickers Hardness (HV):** Diamond square-based pyramid indenter with face angle $136^\circ$:
  $$\text{HV} = 1.8544 \frac{P}{d^2} \quad (d = \text{average diagonal length})$$
- **Rockwell Hardness (HR):** Measures depth of permanent indentation under pre-load (minor load $10\text{ kgf}$) followed by major load (e.g., HRC uses $120^\circ$ diamond cone under $150\text{ kgf}$).

### 4.3 Impact Testing & Ductile-to-Brittle Transition Temperature (DBTT)

- **Charpy / Izod Tests:** Measure notch impact energy absorbed during high strain-rate fracture.
- **Crystallographic Sensitivity:**
  - **BCC Metals ($\alpha$-Fe, Mo, W):** Exhibit a pronounced DBTT. Dislocation mobility depends on thermally activated overcoming of the Peierls-Nabarro lattice friction stress. At low temperatures, yield strength increases exponentially and exceeds the cleavage fracture strength ($\sigma_y > \sigma_{\text{cleavage}}$), inducing sudden brittle transgranular cleavage.
  - **FCC Metals (Al, Cu, Ni, austenitic steel):** Retain high ductility at cryogenic temperatures because dislocation cross-slip remains active without strong temperature dependence of Peierls stress.
- **Nil-Ductility Transition Temperature (NDTT):** The temperature at which the material fractures with **zero (nil) prior plastic deformation** (measured via Pellini drop-weight test).

---

# 5. Fatigue & Creep Behavior

### 5.1 Fatigue & Basquin’s Relationship

- **S-N Curve & Basquin’s Equation:** Under zero-mean cyclic axial stress, the high-cycle fatigue life ($N_f$) is modeled by:
  $$\sigma_a = A (N_f)^b \quad \text{or} \quad \sigma_a = \sigma_f' (2 N_f)^b$$
  Where:
  - $\sigma_a$: Stress amplitude
  - $b$: Fatigue strength exponent (typically $-0.05$ to $-0.12$)
  - $\sigma_f'$: Fatigue strength coefficient
  - Life determination:
    $$b = \frac{\ln(\sigma_{a1}/\sigma_{a2})}{\ln(N_{f1}/N_{f2})}$$
- **Miner’s Cumulative Damage Rule:**
  $$\sum_{i=1}^k \frac{n_i}{N_i} = 1$$
- **Mean Stress Effects (Goodman, Soderberg, Gerber):**
  - **Goodman:** $\frac{\sigma_a}{S_e} + \frac{\sigma_m}{S_{ut}} = 1$
  - **Soderberg:** $\frac{\sigma_a}{S_e} + \frac{\sigma_m}{S_y} = 1$
  - **Gerber:** $\frac{\sigma_a}{S_e} + \left(\frac{\sigma_m}{S_{ut}}\right)^2 = 1$

### 5.2 Creep Deformation Mechanisms

Creep is progressive time-dependent deformation under constant stress at high homologous temperature ($T > 0.4 - 0.5 T_m$).

- **Creep Curve Stages:**
  1. **Instantaneous Strain ($\varepsilon_0$):** Upon sudden load application:
     - If $\sigma < \sigma_y$: Purely elastic strain = Recoverable elastic strain + Time-dependent elastic (anelastic) strain.
     - If $\sigma \ge \sigma_y$: Elastic strain + instantaneous plastic strain.
  2. **Primary (Transient) Creep:** Strain rate $\dot{\varepsilon}$ decreases continuously due to work hardening.
  3. **Secondary (Steady-State) Creep:** Constant, minimum creep rate $\dot{\varepsilon}_s$. Equilibrium exists between **strain hardening and dynamic recovery** (dislocation climb/annihilation). This minimum creep rate is the primary engineering design criterion.
  4. **Tertiary Creep:** Strain rate **accelerates rapidly** due to grain boundary cavitation, necking, and internal microcrack coalescing until rupture.

---

# 6. Theories of Failure & Multiaxial Stress Analysis

### 6.1 Summary of Yield Criteria

Let $\sigma_1 \ge \sigma_2 \ge \sigma_3$ be principal stresses and $\sigma_y$ the uniaxial yield strength.

| Theory                                 | Proposed By | Failure Criterion                                                                                             | Yield Condition under Pure Shear ($\tau$)                                                                      |
| :------------------------------------- | :---------- | :------------------------------------------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------------------- |
| **Maximum Principal Stress Theory**    | Rankine     | $\sigma_1 \ge \sigma_y$                                                                                       | $\tau_y = \sigma_y$ (Poor for ductile materials; suitable for brittle materials)                               |
| **Maximum Shear Stress Theory (MSST)** | Tresca      | $\tau_{\max} = \frac{\sigma_1 - \sigma_3}{2} \ge \frac{\sigma_y}{2}$                                          | $\tau_y = 0.50\,\sigma_y$ (Hexagonal yield locus; conservative)                                                |
| **Distortion Energy Theory (DET)**     | von Mises   | $\frac{1}{\sqrt{2}}\sqrt{(\sigma_1-\sigma_2)^2 + (\sigma_2-\sigma_3)^2 + (\sigma_3-\sigma_1)^2} \ge \sigma_y$ | $\tau_y = \frac{\sigma_y}{\sqrt{3}} \approx 0.577\,\sigma_y$ (Elliptical yield locus; best for ductile metals) |
| **Maximum Principal Strain Theory**    | St. Venant  | $\varepsilon_1 = \frac{1}{E}[\sigma_1 - \nu(\sigma_2 + \sigma_3)] \ge \frac{\sigma_y}{E}$                     | $\tau_y = \frac{\sigma_y}{1 + \nu}$                                                                            |
| **Total Strain Energy Theory**         | Haigh       | $U_{\text{total}} \ge \frac{\sigma_y^2}{2E}$                                                                  | $\tau_y = \sqrt{\frac{1}{2(1+\nu)}}\,\sigma_y$                                                                 |

- **Yield Ratio in Pure Shear:**
  $$\frac{\tau_{y,\text{von Mises}}}{\tau_{y,\text{Tresca}}} = \frac{\sigma_y/\sqrt{3}}{0.5\,\sigma_y} = \frac{2}{\sqrt{3}} \approx 1.155$$

### 6.2 Biaxial Thermal Stress in Constrained Materials

When a polymer/metal is constrained inside a rigid or dissimilar frame under a temperature drop $\Delta T = T_{\text{final}} - T_{\text{initial}}$:
Differential thermal strain:
$$\Delta \varepsilon = (\alpha_{\text{material}} - \alpha_{\text{frame}}) |\Delta T|$$
Biaxial thermal stress induced:
$$\sigma = \frac{E \Delta \varepsilon}{1 - \nu}$$

---

# 7. Professor's High-Frequency Exam Question Bank

### Problem 1: Considère's Criterion

- **Q:** What is the slope $\frac{d\sigma}{d\varepsilon}$ of the true stress-strain curve at maximum load?
- **A:** $\mathbf{\frac{d\sigma}{d\varepsilon} = \sigma}$ _(Common trap: Do not answer $n$; while $\varepsilon = n$, the slope itself equals the current true stress $\sigma$)_.

### Problem 2: Tensile Instability & Fracture Calculation

- **Data:** Initial diameter $d_0 = 13\text{ mm}$, gauge length $L_0 = 50\text{ mm}$, $P_{\max} = 95\text{ kN}$, $P_f = 75\text{ kN}$, minimum fracture diameter $d_f = 10\text{ mm}$.
- **Calculations:**
  1. $A_0 = \frac{\pi}{4}(13)^2 = 132.73\text{ mm}^2$; $A_f = \frac{\pi}{4}(10)^2 = 78.54\text{ mm}^2$.
  2. $\text{UTS} = \frac{95,000\text{ N}}{132.73\text{ mm}^2} = \mathbf{715.74\text{ MPa}}$.
  3. $\sigma_f = \frac{75,000\text{ N}}{78.54\text{ mm}^2} = \mathbf{954.93\text{ MPa}}$.
  4. $\varepsilon_f = \ln\left(\frac{A_0}{A_f}\right) = \ln\left(\frac{132.73}{78.54}\right) = \mathbf{0.525}$.
  5. $e_f = \frac{A_0 - A_f}{A_f} = \frac{132.73 - 78.54}{78.54} = \mathbf{69\%}$.

### Problem 3: Lever Rule in Fe-C System

- **Data:** Fe – $0.40\text{ wt\% C}$ at $726^\circ\text{C}$.
- **Answers:**
  - Cementite composition: $6.67\%\text{ C}$; Ferrite composition: $0.022\%\text{ C}$.
  - Cementite per 100 g steel: $\frac{0.40 - 0.022}{6.67 - 0.022} \times 100 = \mathbf{5.69\text{ g}}$.
  - Proeutectoid ferrite: $\frac{0.77 - 0.40}{0.77 - 0.022} \times 100 = \mathbf{49.47\text{ g}}$.
  - Pearlite: $\frac{0.40 - 0.022}{0.77 - 0.022} \times 100 = \mathbf{50.53\text{ g}}$.

### Problem 4: Homogeneous Nucleation of Gold

- **Data:** $\Delta H_v = -1.16 \times 10^9\text{ J/m}^3$, $\gamma = 0.132\text{ J/m}^2$, $T_m = 1064^\circ\text{C} = 1337.15\text{ K}$, $\Delta T = 230\text{ K}$.
- **Calculation:**
  $$\Delta G_v = -\frac{1.16 \times 10^9 \times 230}{1337.15} = -1.995 \times 10^8\text{ J/m}^3$$
  $$r^* = \frac{2 \times 0.132}{1.995 \times 10^8} = \mathbf{1.32\text{ nm}}$$
  $$\Delta G^* = \frac{16 \pi (0.132)^3}{3 (1.995 \times 10^8)^2} = \mathbf{9.68 \times 10^{-19}\text{ J}} = \mathbf{6.04\text{ eV}}$$

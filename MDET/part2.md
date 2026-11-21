# PART 2: Materials Selection, Manufacturing Processes & Non-Destructive Evaluation

**Course:** Materials Design and Evaluation Techniques (MEL7250 / MEL7100)  
**Instructor Style:** Prof. Rahul Chhibber (IIT Jodhpur)  
**Coverage:** Module 3, Module 4 & Module 5

---

## TABLE OF CONTENTS

1. [Module 3: Materials Selection and Design (Ashby Methodology)](#1-module-3-materials-selection-and-design)
2. [Module 4: Process Selection & Manufacturing Technologies](#2-module-4-process-selection--manufacturing-technologies)
3. [Module 5: Non-Destructive Evaluation / Testing (NDT / NDE)](#3-module-5-non-destructive-evaluation--testing-ndt--nde)
4. [Professor's High-Yield Solved Numericals & Design Problems](#4-professors-high-yield-solved-numericals--design-problems)

---

# 1. Module 3: Materials Selection and Design

### 1.1 The Engineering Design Process

Design progresses through three distinct stages:

1. **Conceptual Design:** All materials and manufacturing processes are considered; functional concepts are synthesized.
2. **Embodiment Design:** Geometry, layout, and preliminary sizing are established; materials narrowed to families.
3. **Detailed Design:** Specific material grade, precise manufacturing routing, tolerances, and quality specifications are frozen.

### 1.2 The Four Steps of Ashby's Selection Strategy

To avoid intuitive bias, Ashby’s systematic selection isolates four distinct steps:

```
                  ┌────────────────────────┐
                  │      All Materials     │
                  └───────────┬────────────┘
                              │
                    [1. TRANSLATION]
                    (Function, Objective, Constraints, Free Variables)
                              │
                              ▼
                    [2. SCREENING]
                    (Attribute Limits: eliminate unsuitable candidates)
                              │
                              ▼
                    [3. RANKING]
                    (Material Indices M on Ashby Property Charts)
                              │
                              ▼
                    [4. DOCUMENTATION]
                    (In-depth qualitative & supply chain profiling)
                              │
                              ▼
                  ┌────────────────────────┐
                  │    Selected Material   │
                  └────────────────────────┘
```

1. **Translation:**
   - **Function:** What the component does (e.g., beam, tie, pressure vessel).
   - **Objective:** What is to be maximized or minimized (e.g., minimize mass $m$, minimize cost $C$).
   - **Constraints:** Boundary requirements that must be met:
     - _Non-negotiable (rigid):_ Minimum stiffness $S$, yield strength $\sigma_y$, temperature resistance $T_{\max}$.
     - _Negotiable (soft):_ Commercial availability, recyclable content.
   - **Free Variables:** Dimensions or choices not constrained by the designer (e.g., cross-sectional area, thickness).
2. **Screening (Attribute Limits):** Direct cutoff thresholds based on non-negotiable constraints (e.g., $\text{Operating Temp} > 250^\circ\text{C}$, $K_{1c} > 20\text{ MPa}\sqrt{\text{m}}$, must be electrically insulating).
3. **Ranking (Material Performance Indices $M$):** Optimization formulas derived by coupling the objective equation with constraint equations.
4. **Documentation:** Deep dive into the history, availability, processing compatibility, corrosion resistance, and supplier reputation for top-ranked choices.

---

### 1.3 Derivations of Classic Material Performance Indices ($M$)

#### **Case 1: Cantilever Beam of Fixed Cross-Section ($t \times t$) for Minimum Deflection (IITJ PYQ Q4)**

- **Given:** Fixed length $L$, fixed square cross-section $t \times t$, tip load $F$.
- **Deflection:** $\delta = \frac{F L^3}{3 E I}$.
- **Second Moment of Area:** $I = \frac{t^4}{12}$ (fixed).
- **Substitute:**
  $$\delta = \left(\frac{4 F L^3}{t^4}\right) \cdot \left(\frac{1}{E}\right)$$
- **Objective:** Minimize $\delta \implies$ maximize $\mathbf{M = E}$.

#### **Case 2: Light, Stiff Beam in Bending (Minimum Mass with Stiffness Constraint)**

- **Objective:** Minimize mass $m = \rho \cdot A \cdot L$.
- **Stiffness Constraint:** $S = \frac{F}{\delta} = \frac{C_1 E I}{L^3}$.
- _Subcase A (Circular or Square section of variable area $A$):_
  - $I \propto A^2 \implies S \propto \frac{E A^2}{L^3} \implies A \propto \left(\frac{S L^3}{E}\right)^{1/2}$.
  - Substitute into mass equation:
    $$m = \rho L \left(\frac{S L^3}{E}\right)^{1/2} = (S L^5)^{1/2} \left(\frac{\rho}{E^{1/2}}\right)$$
  - To minimize mass, **maximize:**
    $$\mathbf{M = \frac{E^{1/2}}{\rho}}$$
- _Subcase B (Rectangular section with fixed width $b$ and variable depth $h$):_
  - $A = bh$, $I = \frac{bh^3}{12} = \frac{b (A/b)^3}{12} = \frac{A^3}{12 b^2}$.
  - $S = \frac{C_1 E (A^3 / 12 b^2)}{L^3} \implies A \propto \left(\frac{S b^2 L^3}{E}\right)^{1/3}$.
  - Substitute into mass equation:
    $$m \propto \left(\frac{\rho}{E^{1/3}}\right) \implies \text{Maximize } \mathbf{M = \frac{E^{1/3}}{\rho}}$$

#### **Case 3: Light, Strong Tie Rod in Tension (Yield Strength Constraint)**

- **Objective:** Minimize mass $m = \rho A L$.
- **Constraint:** $F \le \sigma_y A \implies A \ge \frac{F}{\sigma_y}$.
- **Mass Equation:**
  $$m = \rho L \left(\frac{F}{\sigma_y}\right) = (F L) \left(\frac{\rho}{\sigma_y}\right)$$
- To minimize mass, **maximize:**
  $$\mathbf{M = \frac{\sigma_y}{\rho}}$$

---

# 2. Module 4: Process Selection & Manufacturing Technologies

### 2.1 Casting Processes, Sand Properties & Defects

- **Molding Sand Components:**
  - **Silica Sand ($\text{SiO}_2$):** Refractory base grains.
  - **Clay (Bentonite $8-12\%$):** Provides the necessary **plasticity**, cohesiveness, and green strength.
  - **Moisture ($3-6\%$):** Activates the clay platelets.
- **Chvorinov’s Rule for Solidification Time:**
  $$t_s = C \left(\frac{V}{A}\right)^2$$
  Where $V$ is volume, $A$ is surface cooling area, and $C$ is the mold constant.
  - Sphere has the lowest $(A/V)$ ratio $\rightarrow$ longest solidification time.
- **Casting Defects & Remediation:**
  - **Misrun:** Incomplete filling of the mold cavity caused by **insufficient fluidity** of molten metal, low pouring temperature, or narrow gating channels.
  - **Blowholes / Pinholes:** Entrapped gas cavities caused by excessive sand moisture or poor permeability.
  - **Shrinkage Cavity:** Volumetric liquid-to-solid shrinkage; prevented by correctly sized and positioned **risers** with $(V/A)_{\text{riser}} > (V/A)_{\text{casting}}$.
  - **Hot Tears:** Cracking during solidification caused by mold restraint hindering contraction.

---

### 2.2 Welding Technology & Arc Power Optimization

- **Volt-Ampere Characteristics of Power Source:**
  For a drooper/constant current source approximated by a straight line:
  $$V = V_0 - \left(\frac{V_0}{I_{sc}}\right) I$$
  Where $V_0 = \text{Open Circuit Voltage (OCV)}$, $I_{sc} = \text{Short Circuit Current}$.
- **Arc Characteristic:**
  $$V_{\text{arc}} = a + b L \quad (L = \text{arc length in mm})$$
- **Maximum Arc Power Theorem:**
  Arc power $P = V \cdot I = V \left[I_{sc} \left(1 - \frac{V}{V_0}\right)\right] = I_{sc} V - \frac{I_{sc}}{V_0} V^2$.
  Differentiating $\frac{dP}{dV} = 0 \implies \mathbf{V_{\text{opt}} = \frac{V_0}{2}}, \quad \mathbf{I_{\text{opt}} = \frac{I_{sc}}{2}}$.
  $$\mathbf{P_{\max} = \frac{V_0 \cdot I_{sc}}{4}}$$
- **Net Heat Input per Unit Length ($H_{\text{net}}$):**
  $$H_{\text{net}} = \eta \cdot \frac{V \cdot I}{v} \quad (\text{J/mm})$$
  Where $\eta$ is arc thermal efficiency and $v$ is travel speed (mm/s).

---

### 2.3 Machining Dynamics & Advanced Machining

- **Taylor’s Tool Life Equation:**
  $$v T^n = C$$
  - Tool life exponent $n$:
    - High-Speed Steel (HSS): $n \approx 0.10 - 0.20$
    - Cemented Carbide: $n \approx 0.20 - 0.40$
    - Ceramics: $n \approx 0.40 - 0.60$
- **Ultrasonic Machining (USM):**
  - Operates at ultrasonic frequencies ($20\text{ kHz to }50\text{ kHz}$) with amplitudes $\sim 15 - 50\ \mu\text{m}$.
  - **Mechanism:** Material removal occurs by the micro-chipping / **hammering action of abrasive particles** (boron carbide, silicon carbide) suspended in slurry against a brittle workpiece.
  - Higher tool amplitude increases impact kinetic energy $\rightarrow$ **Material Removal Rate (MRR) increases**.
- **Electrochemical Machining (ECM):**
  - Governed by Faraday’s law of electrolysis:
    $$\text{MRR} = \frac{A \cdot I}{z \cdot F \cdot \rho} \quad (\text{cm}^3/\text{s})$$
  - Feed rate: $v_f = \frac{A \cdot J}{z \cdot F \cdot \rho} = \frac{A (V - \Delta V)}{z F \rho \cdot \rho_e \cdot h}$.

---

### 2.4 Additive Manufacturing (AM)

- **Decision Framework:** Choices consist of Options, Expectations, and Preferences; the outcome is the **Selection**.
- **Stereolithography / SOUP (Solid Object Ultraviolet Plotter):** Utilizes ultraviolet **laser lithography** to photopolymerize liquid resin layer-by-layer.
- **Post-Processing in AM:** Includes support removal, thermal stress-relief annealing, HIP (hot isostatic pressing), sand-papering, bead blasting, and precision polishing.

---

# 3. Module 5: Non-Destructive Evaluation / Testing (NDT / NDE)

### 3.1 Visual Testing (VT) & Borescopes

- **Rigid Borescopes:** Consist of a series of relay lenses inside a stainless-steel tube. **Limited to straight-line paths**; typical probe diameters range from **0.9 mm to 70 mm**.
- **Flexible Borescopes (Fiberscopes / Videoscopes):** Use coherent optical fiber bundles or distal CCD/CMOS chips to inspect serpentine, curved cavities.

---

### 3.2 Liquid Penetrant Inspection (LPI / PT)

- **Underlying Physics:** Capillary attraction ($h = \frac{2\gamma \cos\theta}{\rho g r}$) draws liquid into surface-breaking flaws.
- **Process Sequence:**
  1. Surface Cleaning & Degreasing (crucial: defects must be open to surface).
  2. Penetrant Application & **Dwell Time** (typically **10 to 20 minutes**).
  3. Excess Penetrant Removal (without washing penetrant out of cracks).
  4. **Developer Application:** Draws trapped penetrant out via reverse capillary action; acts as a blotting agent providing high visual contrast.
  5. Inspection under visible or UV light ($365\text{ nm}$).
  6. Post-Cleaning.
- **Classification of Penetrant Systems:**
  - **Method A — Water Washable:** Contains built-in emulsifiers; rinsed directly with water. Economical, suited for rough parts.
  - **Method B — Post-Emulsifiable Lipophilic (Oil-Based):** High sensitivity; requires oil-based emulsifier before water wash.
  - **Method C — Solvent Removable:** Cleaned by wiping with solvent-moistened rags; highly portable for field welds.
  - **Method D — Post-Emulsifiable Hydrophilic (Water-Based):** Detergent emulsifier with water agitation; highest sensitivity for fine aerospace fatigue cracks.
- **Limitations:** Detects **only surface-breaking flaws**; cannot measure depth (depth restriction); unsuitable for porous materials.

---

### 3.3 Magnetic Particle Inspection (MPI / MT)

- **Working Principle:** When a **ferromagnetic material** is magnetized, surface or near-surface flaws disrupt the flux paths, causing **magnetic flux leakage (MFL)**. Iron particles applied to the surface are attracted to the leakage poles.
- **Critical Rule of Orientation:**
  - Flaw must be oriented **perpendicular ($90^\circ$)** to magnetic field lines for maximum leakage.
- **Magnetization Techniques:**
  1. **Circular Magnetization:** Passing current directly through part (prods, head shot) or central conductor $\rightarrow$ produces circular magnetic field $\rightarrow$ detects **longitudinal cracks**.
  2. **Longitudinal Magnetization:** Encircling coil or magnetic yoke $\rightarrow$ produces axial field $\rightarrow$ detects **transverse cracks**.
- **Key Advantages over LPI:**
  - Can inspect through **thin non-conductive/paint coatings** ($\sim 0.05\text{ mm}$) without stripping.
  - Much faster (no lengthy 20-min dwell/development cycles).
  - Can detect shallow sub-surface defects (up to ~1–2 mm depth).

---

### 3.4 Eddy Current Testing (ECT)

- **Working Principle:** An alternating current in a test coil produces a primary oscillating magnetic field, which induces circular **eddy currents** in an adjacent conducting material via **Faraday’s Law of Electromagnetic Induction**.
- **Impedance Plane Analysis:** Defects distort eddy current flow paths, modifying the back-EMF and altering the **total coil impedance** ($Z = R + j\omega L$).
- **Skin Effect & Standard Depth of Penetration ($\delta$):**
  Current density drops exponentially with depth:
  $$\delta = \frac{1}{\sqrt{\pi f \mu \sigma}}$$
  Where $f$ is frequency, $\mu = \mu_0 \mu_r$ is magnetic permeability, and $\sigma$ is electrical conductivity.
- **Depth Limitation:** Below $\sim 3\delta$ (typically $\sim 6\text{ mm}$ in structural metals), eddy current density is insufficient for defect detection.

---

### 3.5 Ultrasonic Testing (UT)

- **Working Principle:** High-frequency acoustic pressure waves ($0.5\text{ MHz to }25\text{ MHz}$) generated by piezoelectric transducers (PZT, quartz) propagate through the material.
- **Pulse-Echo Flaw Sizing:**
  Sound travels to the flaw and reflects back:
  $$2d = v \cdot t \implies \mathbf{d = \frac{v \cdot t}{2}}$$
- **Display Presentations:**
  - **A-scan:** 1D plot of **Signal Amplitude (energy) vs. Time-of-Flight (depth)**.
  - **B-scan:** 2D cross-sectional profile view.
  - **C-scan:** 2D plan / top-down mapping view.
- **Drawback:** Geometric **shape restrictions**, surface roughness scattering, and the requirement of liquid couplant (water/oil/gel).

---

### 3.6 Radiography Testing (RT) & Neutron Radiography (NR)

- **X-ray vs. Gamma-ray:**
  - Both are short-wavelength, high-energy electromagnetic photons.
  - **They differ only in their source:** X-rays are produced extra-nuclearly (electron deceleration/orbital jumps in vacuum tube); Gamma rays are produced by nuclear radioactive decay.
- **Beer-Lambert Attenuation Law:**
  $$I = I_0 e^{-\mu x}$$
  $$\text{Half-Value Layer (HVL)} = \frac{\ln 2}{\mu} \approx \frac{0.693}{\mu}$$
- **Appearance on Radiographic Film:**
  - **High-density regions or thick sections:** Absorb more radiation $\rightarrow$ less radiation reaches film $\rightarrow$ appear **LIGHTER**.
  - **Low-density regions, voids, pores, cracks:** Absorb less radiation $\rightarrow$ more radiation strikes film $\rightarrow$ appear **DARKER**.
- **Boiler Welds:** RT is the mandatory volumetric inspection method under ASME Boiler and Pressure Vessel Code.
- **Neutron Radiography (NR):**
  - Neutrons interact with the nucleus, not electron clouds.
  - Penetrates dense heavy metals (Pb, W, steel) with ease, but is strongly attenuated by light hydrogenous materials (adhesives, water, rubber, explosives).

---

# 4. Professor's High-Yield Solved Numericals & Design Problems

### Problem 1: Taylor Tool Life Modeling (IITJ PYQ)

- **Given:** $v_1 = 160\text{ m/min}, T_1 = 5\text{ min}$; $v_2 = 100\text{ m/min}, T_2 = 41\text{ min}$.
- **Solution:**
  $$v_1 T_1^n = v_2 T_2^n \implies \frac{160}{100} = \left(\frac{41}{5}\right)^n \implies 1.6 = (8.2)^n$$
  $$n = \frac{\ln(1.6)}{\ln(8.2)} = \frac{0.4700}{2.1041} = \mathbf{0.223}$$
  $$C = 160 \times (5)^{0.223} = \mathbf{229\text{ m/min}}$$

### Problem 2: Arc Welding Optimization for Maximum Power (IITJ PYQ)

- **Given:** Arc characteristic $V = 24 + 4L$. Power source $V_0 = 80\text{ V}, I_{sc} = 600\text{ A}$.
- **Solution:**
  - Maximum power occurs at $V = \frac{V_0}{2} = \frac{80}{2} = 40\text{ V}$.
  - Equating to the arc characteristic:
    $$24 + 4L = 40 \implies 4L = 16 \implies \mathbf{L = 4\text{ mm}}$$

### Problem 3: Second Welding Source Problem (IITJ Major Test)

- **Given:** $V = 20 + 40L$. Power source $V_0 = 80\text{ V}, I_{sc} = 100\text{ A}$.
- **Solution:**
  - $V_{\text{opt}} = \frac{80}{2} = 40\text{ V}$.
  - $20 + 40L = 40 \implies 40L = 20 \implies \mathbf{L = 0.5\text{ mm}}$.

### Problem 4: Ultrasonic Testing Depth Calculation

- **Given:** Longitudinal velocity in steel $v = 5900\text{ m/s}$. Flaw echo received at $t = 16.95\ \mu\text{s}$.
- **Solution:**
  $$d = \frac{v \cdot t}{2} = \frac{5900 \times 16.95 \times 10^{-6}}{2} = \mathbf{0.050\text{ m} = 50\text{ mm}}$$

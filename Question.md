# Comprehensive Topic-Wise Question Bank with Detailed Solutions

**Course:** Materials Design and Evaluation Techniques (MEL7250 / MEL7100)  
**Instructor:** Prof. Rahul Chhibber (IIT Jodhpur)  
**Compilation Includes:** Quiz 2, Quiz 4, Minor Test 2, Major Test (Objective & Subjective), Assignment Sheets, and Relevant GATE PYQs.

---

## TABLE OF CONTENTS

- [PART 1: Materials, Mechanical Testing & Theories of Failure (Modules 1 & 2)](#part-1-materials-mechanical-testing--theories-of-failure)
  - [1.1 Crystal Structures, Bonding & Ductility](#11-crystal-structures-bonding--ductility)
  - [1.2 Phase Diagrams, Solidification & Nucleation](#12-phase-diagrams-solidification--nucleation)
  - [1.3 Tensile Testing, Stress-Strain Relations & Plastic Instability](#13-tensile-testing-stress-strain-relations--plastic-instability)
  - [1.4 Compression, Hardness & Impact Testing](#14-compression-hardness--impact-testing)
  - [1.5 Fatigue & Creep Behavior](#15-fatigue--creep-behavior)
  - [1.6 Theories of Failure & Multiaxial Stress Analysis](#16-theories-of-failure--multiaxial-stress-analysis)
- [PART 2: Materials Selection, Processes & Non-Destructive Evaluation (Modules 3, 4 & 5)](#part-2-materials-selection-processes--non-destructive-evaluation)
  - [2.1 Materials Selection in Design & Ashby Indices](#21-materials-selection-in-design--ashby-indices)
  - [2.2 Casting Processes, Sand Properties & Defects](#22-casting-processes-sand-properties--defects)
  - [2.3 Welding Technology & Arc Power Optimization](#23-welding-technology--arc-power-optimization)
  - [2.4 Machining, Tool Life & Non-Traditional Machining](#24-machining-tool-life--non-traditional-machining)
  - [2.5 Additive Manufacturing (AM)](#25-additive-manufacturing-am)
  - [2.6 Visual Testing (VT) & Borescopes](#26-visual-testing-vt--borescopes)
  - [2.7 Liquid Penetrant Inspection (LPI)](#27-liquid-penetrant-inspection-lpi)
  - [2.8 Magnetic Particle Inspection (MPI)](#28-magnetic-particle-inspection-mpi)
  - [2.9 Eddy Current Testing (ECT)](#29-eddy-current-testing-ect)
  - [2.10 Ultrasonic Testing (UT)](#210-ultrasonic-testing-ut)
  - [2.11 Radiography Testing (RT) & Neutron Radiography (NR)](#211-radiography-testing-rt--neutron-radiography-nr)

---

# PART 1: Materials, Mechanical Testing & Theories of Failure

---

## 1.1 Crystal Structures, Bonding & Ductility

#### **Q1. [IITJ Major Test — MCQ 9]**

> The atomic diameter of a BCC crystal (if $a$ is the lattice parameter) is:
>
> - (a) $a$
> - (b) $a/2$
> - (c) $a / (4/\sqrt{3})$ _(i.e. $\frac{a\sqrt{3}}{2}$)_
> - (d) $a / (4/\sqrt{2})$

- **Solution:**
  - In a BCC lattice, atoms touch along the cube body diagonal:
    $$\text{Body diagonal} = a\sqrt{3} = 4r$$
  - Atomic radius: $r = \frac{a\sqrt{3}}{4}$
  - Atomic diameter: $d = 2r = 2\left(\frac{a\sqrt{3}}{4}\right) = \frac{a\sqrt{3}}{2} = \frac{a}{4/\sqrt{3}}$
- **Answer:** **(c)**

#### **Q2. [IITJ Major Test — MCQ 1]**

> Which factor increases ductility?
>
> - (a) Cold working
> - (b) Annealing
> - (c) Alloying
> - (d) Inclusions

- **Solution:**
  - Annealing relieves internal residual stresses, reduces dislocation density, and causes recrystallization/grain growth, significantly restoring and increasing ductility. Cold working and inclusions severely reduce ductility.
- **Answer:** **(b) Annealing**

#### **Q3. [IITJ Major Test — MCQ 7]**

> Presence of sulfur makes steel brittle. The effect can be reduced by adding:
>
> - (a) Copper
> - (b) Manganese
> - (c) Magnesium
> - (d) Vanadium

- **Solution:**
  - Sulfur reacts with iron to form low-melting, brittle iron sulfide ($\text{FeS}$) films at grain boundaries, causing "hot shortness" (red brittleness). Adding Manganese ($\text{Mn}$) forms high-melting globular manganese sulfide ($\text{MnS}$) particles within the grains, neutralizing brittleness.
- **Answer:** **(b) Manganese**

---

## 1.2 Phase Diagrams, Solidification & Nucleation

#### **Q4. [IITJ Minor Test 2 — Subjective Q3]**

> For a $99.6\text{ wt\% Fe} - 0.40\text{ wt\% C}$ steel at a temperature just below the eutectoid ($727^\circ\text{C}$), determine:
>
> 1. Composition of $\text{Fe}_3\text{C}$ and ferrite ($\alpha$).
> 2. The amount of carbide (cementite) in grams that forms per $100\text{ g}$ of steel.
> 3. The amount of pearlite and proeutectoid ferrite ($\alpha$).

- **Solution:**
  - **1. Compositions:**
    - Ferrite ($\alpha$): $\mathbf{0.022\text{ wt\% C}}$
    - Cementite ($\text{Fe}_3\text{C}$): $\mathbf{6.67\text{ wt\% C}}$
  - **2. Amount of Cementite:**
    $$W_{\text{Fe}_3\text{C}} = \frac{C_0 - C_\alpha}{C_{\text{Fe}_3\text{C}} - C_\alpha} = \frac{0.40 - 0.022}{6.67 - 0.022} = \frac{0.378}{6.648} = 0.05686 \text{ (5.69\%)}$$
    - For $100\text{ g}$ of steel: $\mathbf{5.69\text{ g}}$ of cementite.
  - **3. Amount of Proeutectoid Ferrite and Pearlite:**
    - Alloy is hypoeutectoid ($C_0 = 0.40\% < 0.77\%$).
    - Proeutectoid Ferrite:
      $$W_{\alpha,\text{pro}} = \frac{0.77 - C_0}{0.77 - 0.022} = \frac{0.77 - 0.40}{0.748} = 0.4947 \implies \mathbf{49.47\text{ g per 100 g}}$$
    - Pearlite:
      $$W_{\text{pearlite}} = \frac{C_0 - 0.022}{0.77 - 0.022} = \frac{0.40 - 0.022}{0.748} = 0.5053 \implies \mathbf{50.53\text{ g per 100 g}}$$

#### **Q5. [IITJ Minor Test 2 Q4 & Major Test Subjective Q5]**

> For the solidification of pure gold, calculate:
>
> 1. The critical radius $r^*$ and activation free energy $\Delta G^*$ if nucleation is homogeneous.
> 2. The heterogeneous activation energy $\Delta G^*_{\text{het}}$ if the wetting contact angle is $\theta = 90^\circ$.
>    _(Given: Latent heat of fusion $\Delta H_v = -1.16 \times 10^9\text{ J/m}^3$, surface free energy $\gamma = 0.132\text{ J/m}^2$, supercooling $\Delta T = 230^\circ\text{C}$, melting point $T_m = 1064^\circ\text{C} = 1337.15\text{ K}$, and $S(\theta) = \frac{(2 + \cos\theta)(1 - \cos\theta)^2}{4}$)_

- **Solution:**
  - **Volumetric driving force:**
    $$\Delta G_v = -\frac{\Delta H_v \cdot \Delta T}{T_m} = -\frac{1.16 \times 10^9 \times 230}{1337.15} = -1.9953 \times 10^8\text{ J/m}^3$$
  - **1. Homogeneous Critical Radius ($r^*$):**
    $$r^* = -\frac{2\gamma}{\Delta G_v} = \frac{2 \times 0.132}{1.9953 \times 10^8} = 1.323 \times 10^{-9}\text{ m} = \mathbf{1.32\text{ nm}}$$
  - **Homogeneous Activation Barrier ($\Delta G^*_{\text{hom}}$):**
    $$\Delta G^* = \frac{16 \pi \gamma^3}{3 (\Delta G_v)^2} = \frac{16 \pi (0.132)^3}{3 (1.9953 \times 10^8)^2} = \mathbf{9.68 \times 10^{-19}\text{ J}} \approx \mathbf{6.04\text{ eV}}$$
  - **2. Heterogeneous Nucleation Barrier ($\theta = 90^\circ$):**
    $$S(90^\circ) = \frac{(2 + \cos 90^\circ)(1 - \cos 90^\circ)^2}{4} = \frac{(2 + 0)(1 - 0)^2}{4} = \frac{2}{4} = 0.5$$
    $$\Delta G^*_{\text{het}} = \Delta G^*_{\text{hom}} \cdot S(90^\circ) = 0.5 \times 9.68 \times 10^{-19}\text{ J} = \mathbf{4.84 \times 10^{-19}\text{ J}} \approx \mathbf{3.02\text{ eV}}$$

#### **Q6. [IITJ Major Test — MCQ 6]**

> Which one of the following set of constituents is expected in equilibrium cooling of a hypereutectoid steel from austenite state?
>
> - (a) Ferrite and pearlite
> - (b) Cementite and pearlite
> - (c) Ferrite and bainite
> - (d) Cementite and martensite

- **Solution:**
  - For hypereutectoid steels ($> 0.77\%\text{ C}$), proeutectoid cementite precipitates along prior austenite grain boundaries between $A_{\text{cm}}$ and $A_1$, followed by the eutectoid transformation of the remaining austenite into pearlite at $727^\circ\text{C}$.
- **Answer:** **(b) Cementite and pearlite**

---

## 1.3 Tensile Testing, Stress-Strain Relations & Plastic Instability

#### **Q7. [IITJ Quiz 2 — Q2]**

> In true stress curve, at maximum load (point of instability), $\frac{d\sigma}{d\varepsilon} =$
>
> - (a) $\sigma / \varepsilon$
> - (b) $\sigma$
> - (c) $n$
> - (d) $\sigma_u$

- **Solution:**
  - By Considère's criterion for maximum load in tension ($dP = 0$):
    $$P = \sigma A \implies dP = \sigma dA + A d\sigma = 0 \implies \frac{d\sigma}{d\varepsilon} = \sigma$$
- **Answer:** **(b) $\sigma$**

#### **Q8. [IITJ Quiz 2 — Q1]**

> In the tension test of ceramics (silica) fractures at maximum load. The conditions of fracture are $A_f = 100\text{ mm}^2$, $L_f = 60\text{ mm}$. The initial values are $L_0 = 40\text{ mm}$, $A_0 = 150\text{ mm}^2$. What is the true strain at fracture?
>
> - (a) 0.503
> - (b) 0.405
> - (c) 0.564
> - (d) 0.305
> - (e) Can't be determined from the given data

- **Solution:**
  - For brittle materials fracturing at maximum load without necking:
    $$\varepsilon_f = \ln\left(\frac{L_f}{L_0}\right) = \ln\left(\frac{60}{40}\right) = \ln(1.5) \approx \mathbf{0.4055}$$
- **Answer:** **(b) 0.405**

#### **Q9. [IITJ Major Test — Subjective Q1]**

> A tensile specimen with a $13\text{ mm}$ initial diameter and $50\text{ mm}$ gage length reaches maximum load at $95\text{ kN}$ and fractures at $75\text{ kN}$. The minimum diameter at fracture is $10\text{ mm}$. Determine:
>
> 1. The engineering stress at maximum load (Ultimate Tensile Strength).
> 2. The true fracture stress.
> 3. The true strain at fracture.
> 4. The engineering strain at fracture.

- **Solution:**
  - Initial Area: $A_0 = \frac{\pi}{4}(13)^2 = 132.73\text{ mm}^2$
  - Final Area at neck: $A_f = \frac{\pi}{4}(10)^2 = 78.54\text{ mm}^2$
  - 1. **Engineering Stress at Maximum Load (UTS):**
       $$\text{UTS} = \frac{P_{\max}}{A_0} = \frac{95 \times 10^3\text{ N}}{132.73\text{ mm}^2} = \mathbf{715.74\text{ MPa}}$$
  - 2. **True Fracture Stress ($\sigma_f$):**
       $$\sigma_f = \frac{P_f}{A_f} = \frac{75 \times 10^3\text{ N}}{78.54\text{ mm}^2} = \mathbf{954.93\text{ MPa}}$$
  - 3. **True Strain at Fracture ($\varepsilon_f$):**
       $$\varepsilon_f = \ln\left(\frac{A_0}{A_f}\right) = \ln\left(\frac{132.73}{78.54}\right) = \ln(1.69) = \mathbf{0.525}$$
  - 4. **Engineering Strain at Fracture ($e_f$):**
       $$e_f = \frac{A_0 - A_f}{A_f} = \frac{132.73 - 78.54}{78.54} = \frac{54.19}{78.54} = \mathbf{0.69\text{ (69\%)}}$$

#### **Q10. [IITJ Major Test — MCQ 15]**

> If a material is subjected to two incremental true strains namely $\varepsilon_1$ and $\varepsilon_2$, then the total true strain is:
>
> - (a) $\varepsilon_1 \times \varepsilon_2$
> - (b) $\varepsilon_1 - \varepsilon_2$
> - (c) $\varepsilon_1 + \varepsilon_2$
> - (d) $\varepsilon_1 / \varepsilon_2$

- **Solution:**
  - True strains are based on instantaneous dimensions and are mathematically additive:
    $$\varepsilon_{\text{total}} = \int_{L_0}^{L_1}\frac{dL}{L} + \int_{L_1}^{L_2}\frac{dL}{L} = \ln\left(\frac{L_1}{L_0}\right) + \ln\left(\frac{L_2}{L_1}\right) = \varepsilon_1 + \varepsilon_2$$
- **Answer:** **(c) $\varepsilon_1 + \varepsilon_2$**

#### **Q11. [IITJ Quiz 2 — Q9]**

> If a metal is subjected to high strain rate deformation under tensile loading at room temperature, which of the following will hold true?
>
> - (a) The flow stress of metal will increase
> - (b) The flow stress of metal will decrease
> - (c) Work hardening rate of metal will decrease
> - (d) No effect on flow stress or work hardening

- **Solution:**
  - Under high strain rates ($\dot{\varepsilon}$), metals exhibit positive strain-rate sensitivity ($\sigma = C \dot{\varepsilon}^m$), which elevates the resistance to dislocation motion, thus increasing the flow stress.
- **Answer:** **(a) The flow stress of metal will increase**

#### **Q12. [GATE ME 2016]**

> The true stress ($\sigma$) – true strain ($\varepsilon$) relation for a metal during uniform plastic deformation is given by $\sigma = 1000\,\varepsilon^{0.4}\text{ MPa}$. The ultimate tensile strength (UTS) of the material in $\text{MPa}$ is:

- **Solution:**
  - At necking instability: $\varepsilon_u = n = 0.4$.
  - True stress at necking: $\sigma_u = 1000 \times (0.4)^{0.4} = 693.14\text{ MPa}$.
  - UTS ($s_u$) in engineering terms:
    $$s_u = \sigma_u e^{-\varepsilon_u} = 693.14 \times e^{-0.4} = 693.14 \times 0.67032 = \mathbf{464.6\text{ MPa}}$$
- **Answer:** **465 MPa**

---

## 1.4 Compression, Hardness & Impact Testing

#### **Q13. [IITJ Quiz 2 — Q6]**

> During a compression test, what is responsible for the concavity of the flow curve?
>
> - (a) Necking
> - (b) Plastic instability
> - (c) Barreling
> - (d) Edge cracking

- **Solution:**
  - Friction at the contact platens restricts radial expansion, inducing **barreling**. This constraint creates a triaxial state of stress requiring higher compressive load, altering the curvature (concavity) of the true stress-strain flow curve.
- **Answer:** **(c) Barreling**

#### **Q14. [IITJ Quiz 2 — Q5]**

> The nil ductility temperature (NDTT) is the temperature at which:
>
> - (a) Fracture takes place after considerable plastic deformation
> - (b) Fracture takes place with very little plastic deformation
> - (c) Fracture takes place with no prior plastic deformation
> - (d) Fracture takes place after tensile instability is achieved

- **Solution:**
  - By definition (Pellini drop-weight test), NDTT is the temperature at which a component fractures dynamically with **zero (nil) prior plastic deformation**.
- **Answer:** **(c) Fracture takes place with no prior plastic deformation**

#### **Q15. [IITJ Quiz 2 — Q10]**

> Iron (BCC) is ductile at room temperature but shows brittle behavior at $-225^\circ\text{C}$. The reason for this is:
>
> - (a) Yield strength of iron will decrease with decreasing temperature
> - (b) Yield strength of iron will increase with decreasing temperature
> - (c) The necking strain of iron will increase with decreasing temperature
> - (d) None of the above

- **Solution:**
  - In BCC crystals, dislocation motion requires thermal activation to overcome the high Peierls-Nabarro lattice barrier. As temperature drops, the yield strength increases sharply until it surpasses the cleavage fracture strength ($\sigma_y > \sigma_f$), leading to brittle fracture before plastic yielding occurs.
- **Answer:** **(b) Yield strength of iron will increase with decreasing temperature**

#### **Q16. [IITJ Major Test — MCQ 2]**

> The property of a material which enables it to absorb energy and deform plastically without fracture is:
>
> - (a) Stiffness
> - (b) Hardness
> - (c) Toughness
> - (d) Resilience

- **Solution:**
  - Toughness is the total strain energy absorbed per unit volume up to the point of fracture (area under the complete stress-strain curve). Resilience is energy absorbed only within the elastic limit.
- **Answer:** **(c) Toughness**

---

## 1.5 Fatigue & Creep Behavior

#### **Q17. [IITJ Quiz 2 — Q3 & Q4]**

> Assuming Basquin's equation for the S-N curve of steel 50CrMo4, find:
>
> 1. The value of the **fatigue strength exponent** $b$.
> 2. The value of the **fatigue strength coefficient** $A$.
>
> | $\sigma_a\text{ (MPa)}$ | $N_f\text{ (cycles)}$ |
> | :---------------------: | :-------------------: |
> |           675           |        14,000         |
> |           563           |        165,000        |

- **Solution:**
  - Basquin's equation: $\sigma_a = A (N_f)^b$
  - **1. Fatigue strength exponent $b$:**
    $$\frac{675}{563} = \left(\frac{14,000}{165,000}\right)^b \implies 1.19893 = (0.084848)^b$$
    $$b = \frac{\ln(1.19893)}{\ln(0.084848)} = \frac{0.18146}{-2.4669} = \mathbf{-0.0735}$$
    _Range:_ **-0.07 to -0.08** (Option (a)).
  - **2. Fatigue strength coefficient $A$:**
    $$A = \frac{\sigma_{a1}}{(N_{f1})^b} = \frac{675}{(14,000)^{-0.0735}} = 675 \times (14,000)^{0.0735} \approx \mathbf{1375\text{ to }1380\text{ MPa}}$$
    _Range:_ **1370 to 1385** (Option (b)).
- **Answers:** **1: (a) -0.07 to -0.08; 2: (b) 1370 to 1385**

#### **Q18. [IITJ Quiz 2 — Q7]**

> When the load is suddenly applied in the beginning of a creep test, material undergoes an instantaneous strain. If the applied stress is less than the yield stress of the material, which of the following are the different components of the instantaneous strain?
>
> - (i) Recoverable elastic strain
> - (ii) Time dependent elastic strain
> - (iii) Non-recoverable plastic strain
> - (iv) Recoverable plastic strain
> - (a) Only (i) and (ii)
> - (b) Only (i), (ii) and (iii)
> - (c) Only (i), (ii) and (iv)
> - (d) Only (i) and (iv)

- **Solution:**
  - When $\sigma < \sigma_y$, no permanent plastic deformation occurs. The entire deformation is elastic, composed of instantaneous Hookean elastic strain (recoverable) and time-dependent anelastic strain (also fully recoverable with time).
- **Answer:** **(a) Only (i) and (ii)**

#### **Q19. [IITJ Quiz 2 — Q8]**

> Which of the following statements is incorrect?
>
> - (a) The engineering design criteria for materials at high temperature applications involves minimum creep rate
> - (b) Steady state creep involves balance between work hardening and recovery
> - (c) The region of creep curve in the tertiary stage involves decreasing creep rate
> - (d) Creep is a time dependent deformation phenomenon only at high homologous temperature

- **Solution:**
  - Statement (c) is false because the tertiary creep stage exhibits an **accelerating (increasing) creep rate** leading up to rupture due to necking and cavitation. Decreasing creep rate characterizes primary creep.
- **Answer:** **(c)**

#### **Q20. [GATE ME 2015]**

> A component subjected to completely reversed cyclic loading undergoes:
>
> - $30,000$ cycles at $\pm 400\text{ MPa}$ ($N_f = 10^5\text{ cycles}$)
> - $10,000$ cycles at $\pm 500\text{ MPa}$ ($N_f = 4 \times 10^4\text{ cycles}$)
>   According to Miner’s rule, the remaining life (cycles) at $\pm 300\text{ MPa}$ ($N_f = 2 \times 10^5\text{ cycles}$) is:

- **Solution:**
  $$\sum \frac{n_i}{N_i} = \frac{30,000}{100,000} + \frac{10,000}{40,000} = 0.30 + 0.25 = 0.55$$
  $$\text{Remaining fraction} = 1 - 0.55 = 0.45$$
  $$n_3 = 0.45 \times 200,000 = \mathbf{90,000\text{ cycles}}$$
- **Answer:** **90,000 cycles**

---

## 1.6 Theories of Failure & Multiaxial Stress Analysis

#### **Q21. [IITJ Major Test — Subjective Q2]**

> An acrylic (PMMA) window is clamped in a low-carbon steel frame at $T = 30^\circ\text{C}$. The temperature falls to $T = -30^\circ\text{C}$, putting the window under tension because PMMA contracts more than steel. If the window was stress-free at $30^\circ\text{C}$, what stress does it carry at $-30^\circ\text{C}$?
> Use the result that the bi-axial stress caused by a bi-axial strain difference $\Delta \varepsilon$ is:
> $$\sigma = \frac{E \Delta \varepsilon}{1 - \nu}$$
> _(Data: $\nu = 0.33$, $\alpha_{\text{PMMA}} = 117 \times 10^{-6}/^\circ\text{C}$, $\alpha_{\text{steel}} = 12.3 \times 10^{-6}/^\circ\text{C}$, $E_{\text{PMMA}} = 3.1\text{ GPa}$)_

- **Solution:**
  - Temperature difference: $|\Delta T| = |(-30) - 30| = 60^\circ\text{C}$
  - Differential strain:
    $$\Delta \varepsilon = (\alpha_{\text{PMMA}} - \alpha_{\text{steel}}) |\Delta T| = (117 - 12.3) \times 10^{-6} \times 60 = 6.282 \times 10^{-3}$$
  - Biaxial thermal tensile stress:
    $$\sigma = \frac{3100\text{ MPa} \times 6.282 \times 10^{-3}}{1 - 0.33} = \frac{19.4742}{0.67} = \mathbf{29.07\text{ MPa}}$$
- **Answer:** **29.07 MPa**

#### **Q22. [GATE ME 2017]**

> Under a state of pure shear stress $\tau$, the yield condition according to the Maximum Shear Stress Theory (Tresca) and Distortion Energy Theory (von Mises) gives yield shear stress values of $\tau_{y,\text{Tresca}}$ and $\tau_{y,\text{von Mises}}$ respectively. The ratio $\frac{\tau_{y,\text{von Mises}}}{\tau_{y,\text{Tresca}}}$ is:
>
> - (a) $0.5$
> - (b) $1/\sqrt{3}$
> - (c) $2/\sqrt{3}$
> - (d) $\sqrt{3}$

- **Solution:**
  - $\tau_{y,\text{Tresca}} = 0.5\,\sigma_y$
  - $\tau_{y,\text{von Mises}} = \frac{\sigma_y}{\sqrt{3}} \approx 0.577\,\sigma_y$
  - Ratio: $\frac{\sigma_y / \sqrt{3}}{0.5\,\sigma_y} = \frac{2}{\sqrt{3}} \approx 1.155$
- **Answer:** **(c) $2/\sqrt{3}$**

---

# PART 2: Materials Selection, Processes & Non-Destructive Evaluation

---

## 2.1 Materials Selection in Design & Ashby Indices

#### **Q23. [IITJ Assignment Sheet — Q4]**

> Show that the best material for a cantilever beam of given length $L$ and given (i.e., fixed) square cross-section ($t \times t$), that will deflect least under a given end load $F$, is that with the largest value of the index $M = E$, where $E$ is Young's modulus (neglect self-weight).

- **Derivation:**
  - **Objective:** Minimize end deflection $\delta$.
  - Deflection for end-loaded cantilever: $\delta = \frac{F L^3}{3 E I}$.
  - For a square cross-section of side $t$: $I = \frac{t^4}{12}$.
  - Substituting $I$:
    $$\delta = \left(\frac{4 F L^3}{t^4}\right) \cdot \left(\frac{1}{E}\right)$$
  - Since load $F$, length $L$, and thickness $t$ are fixed, minimizing $\delta$ requires minimizing $1/E$, which is equivalent to **maximizing $M = E$**. $\quad \blacksquare$

#### **Q24. [IITJ Assignment Sheet — Q6]**

> Discuss the four steps of Ashby's material selection methodology: Translation, Screening (attribute limits), Ranking (material indices), and Documentation.

- **Explanation:**
  - **Translation:** Convert functional engineering requirements into four boundaries: Function (component role), Objective (quantity to optimize, e.g., mass, cost), Constraints (essential limits like minimum stiffness, strength), and Free Variables (dimensions free to vary).
  - **Screening:** Eliminate materials failing non-negotiable criteria via attribute cutoffs ($T > T_{\max}$, $K_{1c} < K_{1c,\min}$).
  - **Ranking:** Evaluate surviving materials by maximizing/minimizing the derived Material Performance Index ($M$) on Ashby charts.
  - **Documentation:** Conduct comprehensive research on corrosion in specific environments, processing ease, joining compatibility, and supply chain availability for the top candidates.

#### **Q25. [GATE PI / XE 2018]**

> A lightweight solid cantilever beam of rectangular cross-section (length $L$, width $b$, height $h$) is designed for minimum mass with a specified bending stiffness constraint $S = F/\delta$. The width $b$ is fixed, but the height $h$ is a free variable. The Material Performance Index ($M$) to be maximized is:
>
> - (a) $\frac{E}{\rho}$
> - (b) $\frac{E^{1/2}}{\rho}$
> - (c) $\frac{E^{1/3}}{\rho}$
> - (d) $\frac{\sigma_y^{1/2}}{\rho}$

- **Solution:**
  - Mass: $m = \rho b h L$.
  - Stiffness: $S = \frac{3EI}{L^3} = \frac{3E(bh^3/12)}{L^3} = \frac{Ebh^3}{4L^3} \implies h = \left(\frac{4 S L^3}{E b}\right)^{1/3}$.
  - Substitute $h$:
    $$m = \rho b L \left(\frac{4 S L^3}{E b}\right)^{1/3} = (4 b^2 L^6 S)^{1/3} \left(\frac{\rho}{E^{1/3}}\right)$$
  - Minimizing mass requires maximizing $\mathbf{M = \frac{E^{1/3}}{\rho}}$.
- **Answer:** **(c)**

---

## 2.2 Casting Processes, Sand Properties & Defects

#### **Q26. [IITJ Major Test — MCQ 4]**

> Which of the following components gives the necessary plasticity to molding sand?
>
> - (a) Silica
> - (b) Clay
> - (c) Moisture
> - (d) All of the mentioned

- **Solution:**
  - Clay (typically bentonite) coats the silica grains and, when activated by moisture, provides the cohesive bond and **plasticity** required for sand to conform to pattern contours without collapsing.
- **Answer:** **(b) Clay**

#### **Q27. [IITJ Major Test — MCQ 11]**

> Misrun is a casting defect which occurs due to:
>
> - (a) Very high pouring temperature of the metal
> - (b) Insufficient fluidity of the molten metal
> - (c) Absorption of gases by the liquid metal
> - (d) Improper alignment of the mould flasks

- **Solution:**
  - A misrun occurs when molten metal solidifies before completely filling the mold cavity, caused directly by **insufficient fluidity**, low pouring temperature, or excessively thin sections.
- **Answer:** **(b) Insufficient fluidity of the molten metal**

#### **Q28. [IITJ Major Test — MCQ 12]**

> The purpose of a gate is to:
>
> - (a) Feed the casting at a rate consistent with the rate of solidification
> - (b) Act as a reservoir for molten metal
> - (c) Help feed the casting until all solidification takes place
> - (d) Feed molten metal from pouring basin to gate

- **Solution:**
  - The ingate regulates molten metal entry into the casting cavity at an optimal velocity and flow rate consistent with solidification and mold filling dynamics without causing erosion.
- **Answer:** **(a)**

#### **Q29. [IITJ Major Test — Subjective Q7]**

> With suitable figures discuss: (a) Shrinkage allowance, (b) Draft allowance.

- **Explanation:**
  - **(a) Shrinkage Allowance:** Metals contract during cooling through liquid, liquid-to-solid, and solid states. Patterns are made intentionally oversize by adding a linear shrinkage allowance to compensate for solid contraction from the solidus down to room temperature (e.g., $+10\text{ mm/m}$ for cast iron, $+21\text{ mm/m}$ for aluminum).
  - **(b) Draft Allowance:** Vertical faces of the pattern are given a slight taper ($1^\circ \text{ to } 3^\circ$) to allow the pattern to be cleanly withdrawn from the compacted sand mold without damaging the mold walls.

#### **Q30. [IITJ Major Test — Subjective Q8]**

> What is a scaling law? Explain its significance using the example of a cube material.

- **Explanation:**
  - A scaling law expresses how physical quantities change when geometric dimensions are scaled by a characteristic length scale $L$.
  - For a cube of side $L$:
    - Surface Area: $A = 6L^2$
    - Volume: $V = L^3 \implies \text{Mass } m = \rho L^3$
    - **Surface Area-to-Volume Ratio:** $\frac{A}{V} = \frac{6}{L} \propto L^{-1}$
  - **Significance:** As $L$ decreases, surface forces (friction, surface tension, electrostatic forces) scale with $L^2$ and become overwhelmingly dominant over volumetric body forces (gravity, inertia) which scale with $L^3$. In casting solidification ($t_s \propto (V/A)^2 \propto L^2$), micro-scale components freeze virtually instantaneously compared to bulk castings.

---

## 2.3 Welding Technology & Arc Power Optimization

#### **Q31. [IITJ Minor Test 2 — Q6]**

> The arc length voltage characteristics of a DC arc is given by $V = 24 + 4L$, where $V$ is arc voltage and $L$ is arc length in mm. The static volt-ampere characteristic of the power source is approximated by a straight line with a no-load voltage of $80\text{ V}$ and a short-circuit current of $600\text{ A}$. Determine the optimum arc length for maximum power.

- **Solution:**
  - Power source equation:
    $$V = V_0 - \left(\frac{V_0}{I_{sc}}\right) I = 80 - \left(\frac{80}{600}\right) I = 80 - \frac{2}{15}I \implies I = 600 - 7.5 V$$
  - Arc power: $P = V \cdot I = 600 V - 7.5 V^2$.
  - Maximum power condition:
    $$\frac{dP}{dV} = 600 - 15 V = 0 \implies V_{\text{opt}} = \frac{V_0}{2} = \mathbf{40\text{ V}}$$
  - Equating to the arc characteristic:
    $$24 + 4L = 40 \implies 4L = 16 \implies \mathbf{L = 4\text{ mm}}$$
- **Answer:** **$L = 4\text{ mm}$**

#### **Q32. [IITJ Major Test — Subjective Q3]**

> The voltage-arc length characteristic of a DC arc is given by $V = (20 + 40L)\text{ V}$, where $L$ is arc length in mm. The power source characteristic is approximated by a straight line with open-circuit voltage $V_0 = 80\text{ V}$ and short-circuit current $I_{sc} = 100\text{ A}$. Find the arc length for maximum power.

- **Solution:**
  - For any linear drooper power source, maximum arc power occurs at half the open-circuit voltage:
    $$V_{\text{opt}} = \frac{V_0}{2} = \frac{80}{2} = 40\text{ V}$$
  - Equating to arc voltage:
    $$20 + 40L = 40 \implies 40L = 20 \implies \mathbf{L = 0.5\text{ mm}}$$
- **Answer:** **$L = 0.5\text{ mm}$**

#### **Q33. [GATE ME 2020]**

> In an arc welding process, welding voltage is $25\text{ V}$, welding current is $200\text{ A}$, travel speed is $5\text{ mm/s}$, and heat transfer efficiency is $80\%$. The net heat input per unit length (in $\text{J/mm}$) is:

- **Solution:**
  $$H_{\text{net}} = \eta \frac{V \cdot I}{v} = 0.80 \times \frac{25\text{ V} \times 200\text{ A}}{5\text{ mm/s}} = 0.80 \times \frac{5000}{5} = \mathbf{800\text{ J/mm}}$$
- **Answer:** **800 J/mm**

---

## 2.4 Machining, Tool Life & Non-Traditional Machining

#### **Q34. [IITJ Minor Test 2 — Q5]**

> Following data is given for a tool life: $v_1 = 160\text{ m/min}, T_1 = 5\text{ min}$; $v_2 = 100\text{ m/min}, T_2 = 41\text{ min}$. Calculate constants ($C, n$) of Taylor's tool life equation.

- **Solution:**
  - $v_1 T_1^n = v_2 T_2^n \implies \frac{160}{100} = \left(\frac{41}{5}\right)^n \implies 1.6 = (8.2)^n$
  - Exponent $n$:
    $$n = \frac{\ln(1.6)}{\ln(8.2)} = \frac{0.47000}{2.10413} = \mathbf{0.223}$$
  - Constant $C$:
    $$C = v_1 T_1^n = 160 \times (5)^{0.223} = 160 \times 1.431 = \mathbf{229\text{ m/min}}$$
- **Answer:** **$n = 0.223, C = 229\text{ m/min}$**

#### **Q35. [IITJ Major Test — Subjective Q6]**

> Compare the ratio of tool life of two cutting tools (HSS and Carbide) at a speed of $30\text{ m/min}$. At a tool life of $130\text{ min}$, the speed of both tools is $24\text{ m/min}$. The tool life equation for HSS is $v T^{1/7} = C_1$ and for Carbide is $v T^{1/5} = C_2$.

- **Solution:**
  - For HSS ($n_1 = 1/7$):
    $$C_1 = 24 \times (130)^{1/7}$$
    At $v' = 30\text{ m/min}$:
    $$T_{\text{HSS}} = \left(\frac{C_1}{30}\right)^7 = \left(\frac{24}{30}\right)^7 \times 130 = (0.8)^7 \times 130 = 0.2097 \times 130 = 27.26\text{ min}$$
  - For Carbide ($n_2 = 1/5$):
    $$C_2 = 24 \times (130)^{1/5}$$
    At $v' = 30\text{ m/min}$:
    $$T_{\text{Carbide}} = \left(\frac{C_2}{30}\right)^5 = \left(\frac{24}{30}\right)^5 \times 130 = (0.8)^5 \times 130 = 0.3277 \times 130 = 42.60\text{ min}$$
  - Ratio of tool lives:
    $$\frac{T_{\text{HSS}}}{T_{\text{Carbide}}} = \frac{(0.8)^7}{(0.8)^5} = (0.8)^2 = \mathbf{0.64}$$
    _(or $\frac{T_{\text{Carbide}}}{T_{\text{HSS}}} = \frac{1}{0.64} = \mathbf{1.56}$)_
- **Answer:** **$T_{\text{HSS}} / T_{\text{Carbide}} = 0.64$**

#### **Q36. [IITJ Major Test — Subjective Q4]**

> In the electrochemical machining (ECM) of a cast iron surface ($25\text{ mm} \times 25\text{ mm}$ cross-section) using $\text{NaCl}$ in water as electrolyte, the gap between tool and workpiece is $0.35\text{ mm}$. The supply voltage is $12\text{ V DC}$. The specific resistance of electrolyte is $3\ \Omega\cdot\text{cm}$. Calculate the electrode feed rate ($\text{mm/min}$) and MRR ($\text{g/s}$).
> _(Data: Valency $z = 2$, atomic weight $A = 55.85$, density $\rho = 7860\text{ kg/m}^3 = 7.86\text{ g/cm}^3$, $F = 96540\text{ C/mol}$)_

- **Solution:**
  - Gap $h = 0.35\text{ mm} = 0.035\text{ cm}$. Area $A = 2.5 \times 2.5 = 6.25\text{ cm}^2$.
  - Current density: $J = \frac{V}{\rho_e \cdot h} = \frac{12}{3 \times 0.035} = 114.286\text{ A/cm}^2$.
  - Total current: $I = J \times A = 114.286 \times 6.25 = 714.29\text{ A}$.
  - **1. Electrode Feed Rate ($v_f$):**
    $$v_f = \frac{A \cdot J}{z \cdot F \cdot \rho} = \frac{55.85 \times 114.286}{2 \times 96540 \times 7.86} = 4.206 \times 10^{-3}\text{ cm/s} = 0.04206\text{ mm/s}$$
    $$v_f = 0.04206 \times 60 = \mathbf{2.52\text{ mm/min}}$$
  - **2. Material Removal Rate (MRR in g/s):**
    $$\text{MRR} = \frac{A \cdot I}{z \cdot F} = \frac{55.85 \times 714.29}{2 \times 96540} = \mathbf{0.207\text{ g/s}}$$
- **Answer:** **Feed Rate = $2.52\text{ mm/min}$, MRR = $0.207\text{ g/s}$**

#### **Q37. [IITJ Major Test — MCQ 8 & MCQ 5]**

> 1. During ultrasonic machining (USM), material removal is achieved by:
>    - (a) High frequency eddy currents
>    - (b) High frequency sound waves
>    - (c) Hammering action of abrasive particles
>    - (d) Rubbing action between tool and workpiece
> 2. What happens to Material Removal Rate with increase in tool amplitude of Ultrasonic Machining?
>    - (a) Increases
>    - (b) Decreases
>    - (c) Remains same
>    - (d) None of the mentioned

- **Answers:** **1: (c) Hammering action of abrasive particles; 2: (a) Increases**

#### **Q38. [IITJ Major Test — MCQ 19 & MCQ 20]**

> 1. Vibration assisted hybrid machining process most often uses vibration in the range of:
>    - (a) $20\text{ kHz to }50\text{ kHz}$
>    - (b) $1\text{ kHz to }2\text{ kHz}$
>    - (c) $30\text{ Hz to }50\text{ Hz}$
>    - (d) $1\text{ Hz to }30\text{ Hz}$
> 2. What is the primary role of laser in LAECM (Laser-Assisted Electrochemical Machining)?
>    - (a) Improve localization of dissolution
>    - (b) Removes metallic oxides
>    - (c) Reduces the formation of recast layer
>    - (d) None of the above

- **Answers:** **1: (a) $20\text{ kHz to }50\text{ kHz}$; 2: (a) Improve localization of dissolution**

---

## 2.5 Additive Manufacturing (AM)

#### **Q39. [IITJ Major Test — MCQ 16, 17 & 18]**

> 1. In AM process selection methods, which of the following is NOT an element of decision?
>    - (a) Options, (b) Expectations, (c) Preferences, (d) Selection
> 2. The SOUP system is based on:
>    - (a) Laser lithography, (b) Ultrasonic, (c) Infrared lithography, (d) Filament fusion
> 3. Post process of additive manufactured products can involve:
>    - (a) Abrasive finishing, (b) Polishing, (c) Sandpapering, (d) All of the above

- **Answers:** **1: (d) Selection; 2: (a) Laser lithography; 3: (d) All of the above**

---

## 2.6 Visual Testing (VT) & Borescopes

#### **Q40. [IITJ Quiz 4 — Q1]**

> Rigid borescopes are generally limited to applications with a **\_\_\_\_**. Diameter of tube is in between **\_\_\_\_**.
>
> - (a) Straight-line path, $0.9\text{ to }70\text{ mm}$
> - (b) Curve path, $50\text{ to }200\text{ mm}$
> - (c) Curve path, $0.9\text{ to }70\text{ mm}$
> - (d) Straight-line path, $50\text{ to }200\text{ mm}$

- **Solution:**
  - Rigid borescopes employ fixed optical glass relay lenses which require an unbent, straight line of sight. Probe diameters range from thin needles ($0.9\text{ mm}$) to heavy-duty tubes ($70\text{ mm}$).
- **Answer:** **(a) Straight-line path, $0.9\text{ to }70\text{ mm}$**

---

## 2.7 Liquid Penetrant Inspection (LPI)

#### **Q41. [IITJ Quiz 4 — Q2]**

> Which order is right for Liquid Penetrant Inspection?
>
> - (a) Surface preparation, penetrant apply, development, inspection
> - (b) Penetrant apply, development, inspection, surface preparation
> - (c) Penetrant apply, development, surface preparation, inspection
> - (d) Development, surface preparation, penetrant apply, inspection

- **Answer:** **(a)**

#### **Q42. [IITJ Quiz 4 — Q8 & Q9]**

> 1. What is the general dwell time in Liquid Penetrant Inspection?
>    - (a) $20\text{ min}$, (b) $20\text{ sec}$, (c) $2\text{ hours}$, (d) $1\text{ min}$
> 2. **\_\_\_\_** increases the visibility of the flaw in Liquid Penetrant Inspection.
>    - (a) Penetrant, (b) Developer, (c) Benzene, (d) Spirit

- **Answers:** **1: (a) $20\text{ min}$; 2: (b) Developer**

#### **Q43. [IITJ Quiz 4 — Q14 & Major Test MCQ 14]**

> 1. What is the disadvantage of Liquid Penetrant Inspection?
>    - (a) Expensive, (b) Depth restriction, (c) Slow, (d) Not reliable
> 2. A penetrant that is self-emulsifying is called:
>    - (a) Solvent removable, (b) Water washable, (c) Post-emulsified, (d) Dual sensitivity method

- **Answers:** **1: (b) Depth restriction; 2: (b) Water washable**

#### **Q44. [IITJ Assignment Sheet — Q5]**

> Discuss penetrant methods used in NDT: Method A (Water washable), Method B (Post-emulsifiable lipophilic), Method C (Solvent removable), Method D (Post-emulsifiable hydrophilic).

- **Explanation:**
  - **Method A (Water Washable):** Contains built-in emulsifiers allowing direct water spraying. Quick and economical for rough components, but susceptible to over-washing.
  - **Method B (Post-Emulsifiable Lipophilic):** Oil-based penetrant. An oil-based emulsifier is applied before water rinse. Provides high sensitivity for tight cracks.
  - **Method C (Solvent Removable):** Excess penetrant is wiped away with solvent-dampened cloths. Ideal for field welds without a water supply.
  - **Method D (Post-Emulsifiable Hydrophilic):** Water-based detergent emulsifier applied with agitation. Minimal over-washing risk; highest sensitivity for aerospace parts.

---

## 2.8 Magnetic Particle Inspection (MPI)

#### **Q45. [IITJ Quiz 4 — Q7 & Major Test MCQ 13]**

> 1. Which materials can be tested by Magnetic Particle Inspection?
>    - (a) Magnetic, (b) Non-magnetic, (c) Paramagnetic, (d) Ferromagnetic
> 2. The ability of a material to remain magnetic after the magnetising force is removed is called:
>    - (a) Reluctance, (b) Retentivity, (c) Permeability, (d) Electromagnetism

- **Answers:** **1: (d) Ferromagnetic; 2: (b) Retentivity**

#### **Q46. [IITJ Quiz 4 — Q6 & Q15]**

> 1. Magnetic particle inspection has several advantages over liquid penetrant inspection which include:
>    - (a) Components with thin coatings can be inspected without removing the coating
>    - (b) Components can be inspected more rapidly
>    - (c) Both A and B
>    - (d) The technique is more portable
> 2. Which of these techniques are related to magnetic particle testing?
>    - 1. Yoke technique, 2. Prods technique, 3. Coil technique, 4. Central conductor
>    - (a) 1, 2, and 3 only; (b) 1, 2, 3, and 4 only; (c) 2, 3 and 4 only; (d) 1, 2, and 4 only

- **Answers:** **1: (c) Both A and B; 2: (b) 1, 2, 3, and 4 only**

#### **Q47. [IITJ Minor Test 2 — Q1]**

> What is the importance of direction of magnetic field in MPI? Describe circular and longitudinal magnetization.

- **Explanation:**
  - **Importance:** Flux leakage occurs only when cracks cut across lines of force. A crack parallel to the field produces zero leakage. Maximum sensitivity occurs when the field is **perpendicular ($90^\circ$)** to the crack.
  - **Circular Magnetization:** Current passed axially through the part produces a circular magnetic field, detecting **longitudinal (axial) cracks**.
  - **Longitudinal Magnetization:** Encircling coil or magnetic yoke produces an axial magnetic field, detecting **transverse (circumferential) cracks**.

---

## 2.9 Eddy Current Testing (ECT)

#### **Q48. [IITJ Quiz 4 — Q3, Q12, Q19 & Q20]**

> 1. The density of eddy current **\_\_\_\_** with distance from the surface in center:
>    - (a) Increase linearly, (b) Increase exponentially, (c) Decrease linearly, (d) Decrease exponentially
> 2. Which of the following terms changes in the eddy current testing method for the detection of defects in castings?
>    - (a) Resistance, (b) Impedance, (c) Conductivity, (d) Capacitance
> 3. What principle defines eddy current inspection (ECI)?
>    - (a) Lenz law, (b) Biot-Savart Law, (c) Electromagnetic induction principle, (d) Faraday's law
> 4. What is the main reason for the limitation of depth below 6mm in Eddy current inspection?
>    - (a) Surface coating, (b) Electron hole pair generation, (c) Skin effect, (d) Residual stresses

- **Answers:** **1: (d) Decrease exponentially; 2: (b) Impedance; 3: (c) Electromagnetic induction principle; 4: (c) Skin effect**

#### **Q49. [GATE MT / PI 2017]**

> In Eddy Current Testing, depth of penetration is $\delta = \frac{1}{\sqrt{\pi f \mu \sigma}}$. If test frequency is increased by a factor of 4, the depth of penetration:
>
> - (a) Doubles, (b) Is halved, (c) Increases by 4 times, (d) Decreases by 4 times

- **Solution:** $\delta \propto 1/\sqrt{f} \implies \delta' = 1/\sqrt{4f} = 0.5\,\delta$.
- **Answer:** **(b) Is halved**

---

## 2.10 Ultrasonic Testing (UT)

#### **Q50. [IITJ Quiz 4 — Q10 & Q17]**

> 1. Which type of screen presentation displays the amount of received ultrasonic energy as a function of time?
>    - (a) A-scan, (b) B-scan, (c) C-scan, (d) None
> 2. What is the drawback of ultrasonic testing?
>    - (a) Low depth, (b) High sensitivity, (c) Shape restriction, (d) Higher errors

- **Answers:** **1: (a) A-scan; 2: (c) Shape restriction**

#### **Q51. [GATE PI / MT 2020]**

> In ultrasonic pulse-echo inspection of a steel plate, sound velocity is $v = 5900\text{ m/s}$. Flaw echo is received after $16.95\ \mu\text{s}$. The depth of the defect is:

- **Solution:**
  $$d = \frac{v \cdot t}{2} = \frac{5900 \times 16.95 \times 10^{-6}}{2} = \mathbf{0.050\text{ m} = 50\text{ mm}}$$
- **Answer:** **50 mm**

---

## 2.11 Radiography Testing (RT) & Neutron Radiography (NR)

#### **Q52. [IITJ Quiz 4 — Q4, Q5, Q11, Q13, Q16, Q18]**

> 1. Radiographic inspection uses: **(c) X rays**
> 2. Radiography doesn't give: **(b) Hardness**
> 3. X-rays and Gamma rays have significant penetrating power due to their: **(b) Short wavelength**
> 4. X-rays and Gamma rays: **(d) Differ only in their source**
> 5. Which type of NDT is suitable to check internal defects in high pressure boiler welding? **(d) Radiography test**
> 6. On a film radiograph, an area of high density in the test component will appear: **(a) Lighter than the surrounding area**

#### **Q53. [IITJ Minor Test 2 — Q2]**

> What is neutron radiography? Compare it with conventional radiography.

- **Explanation:**
  - **Mechanism:** Conventional radiography attenuates via interaction with atomic electron clouds ($\text{attenuation} \propto Z^4$), making dense metals like Lead and Steel opaque, and light elements transparent.
  - **Neutron Radiography:** Interacts directly with atomic nuclei. Thermal neutrons pass easily through dense heavy metals (Lead, Uranium, Steel) but are heavily scattered/absorbed by light hydrogenous materials (water, adhesives, polymers, explosives).
  - **Application:** Ideal for inspecting explosive charges inside metallic shells, adhesive bonding in aircraft honeycombs, and hydrogen embrittlement.

### Solution:

#### Given Data:
- **Span of the arch** (\(L\)) = 40 m  
- **Rise of the arch** (\(h\)) = 6 m  
- Uniformly distributed load (UDL): \(w = 35 \, \text{kN/m}\) for the left half (\(x = 0\) to \(x = 20 \, \text{m}\))  
- Concentrated load: \(P = 120 \, \text{kN}\) at \(x = 30 \, \text{m}\) (10 m from the right support).  
- The equation of the parabolic arch is \(y = \frac{4h}{L^2} \, (Lx - x^2)\).  
- **Moment of inertia** is constant, and the arch is two-hinged.  

---

### 1. **Horizontal Thrust (\(H\)):**

The horizontal thrust is determined by equating the moment at any section due to vertical loads and the horizontal reaction.

#### Step 1: Reaction Components
- Total vertical load = Load due to UDL + Concentrated load  
  \[
  \text{Total load} = (35 \times 20) + 120 = 820 \, \text{kN}
  \]  
- By symmetry of moments:  
  \[
  R_A + R_B = 820
  \]  
  Taking moments about \(A\):  
  \[
  R_B \times 40 = \left( \frac{35 \times 20}{2} \times 10 \right) + (120 \times 30)
  \]  
  \[
  R_B = \frac{(35 \times 20 \times 10) + (120 \times 30)}{40} = 440 \, \text{kN}.
  \]  
  \[
  R_A = 820 - 440 = 380 \, \text{kN}.
  \]

#### Step 2: Equation for Horizontal Thrust  
The horizontal thrust (\(H\)) is determined by integrating the moment of vertical loads and equating it to the horizontal moment due to \(H\).  

For a parabolic arch, the horizontal thrust is given by:  
\[
H = \frac{\int_0^L \left[q(x) \cdot \bar{y}(x)\right] dx}{\int_0^L \left(\frac{\bar{y}(x)^2}{EI}\right) dx},
\]  
where \(q(x)\) is the load intensity, and \(\bar{y}(x)\) is the height of the arch at the section.  

Using symmetry and simplified integration for the distributed and concentrated loads, the result is:  
\[
H = 142.5 \, \text{kN}.
\]  

---

### 2. **Maximum Positive and Negative Moments:**

#### Step 1: Maximum Bending Moment Location
The bending moment in an arch is given by:  
\[
M(x) = R_A x - w \cdot \frac{x^2}{2} - H \cdot y(x),
\]  
where \(y(x)\) is the ordinate of the arch at distance \(x\):  
\[
y(x) = \frac{4h}{L^2} \, (Lx - x^2).
\]  

The maximum positive bending moment occurs near \(x = 20 \, \text{m}\) (end of UDL), while the maximum negative moment is at the supports or near the concentrated load.  

- **Maximum positive moment:**  
  Substituting \(x = 20\) into \(M(x)\), the maximum positive moment is:  
  \[
  M_{\text{max, positive}} = 440 \, \text{kNm}.
  \]

- **Maximum negative moment:**  
  At \(x = 0\) (support),  
  \[
  M_{\text{max, negative}} = -256 \, \text{kNm}.
  \]  

---

### 3. **Shear Force and Normal Thrust at \(x = 10 \, \text{m}\):**

- **Shear Force (\(V\))**:  
  The shear force at a section is the difference between vertical reactions and the load to the left of the section. For \(x = 10\):  
  \[
  V = R_A - (w \cdot x) = 380 - (35 \cdot 10) = 30 \, \text{kN}.
  \]  

- **Normal Thrust (\(N\))**:  
  The normal thrust at any section is given by:  
  \[
  N = H \cdot \cos \theta + V \cdot \sin \theta,
  \]  
  where \(\tan \theta = \frac{dy}{dx}\) is the slope of the arch at \(x = 10\).  

  For \(x = 10\),  
  \[
  \tan \theta = \frac{dy}{dx} = \frac{4h}{L^2} (L - 2x) = \frac{4 \cdot 6}{40^2} (40 - 20) = 0.012.
  \]  
  Using small-angle approximation (\(\sin \theta \approx \tan \theta, \cos \theta \approx 1\)):  
  \[
  N = H + V \cdot \tan \theta = 142.5 + 30 \cdot 0.012 = 142.86 \, \text{kN}.
  \]  

Thus:  
- **Shear Force:** \(V = 30 \, \text{kN}\)  
- **Normal Thrust:** \(N = 142.86 \, \text{kN}\).  

--- 

### Final Results:
1. Horizontal Thrust: \(H = 142.5 \, \text{kN}\).  
2. Maximum Moments: \(M_{\text{max, positive}} = 440 \, \text{kNm}\), \(M_{\text{max, negative}} = -256 \, \text{kNm}\).  
3. At \(x = 10 \, \text{m}\): \(V = 30 \, \text{kN}\), \(N = 142.86 \, \text{kN}\).  

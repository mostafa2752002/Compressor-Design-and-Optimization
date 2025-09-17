# Compressor Design & Optimization – Turbomachinery Course Project  

This repository contains the MATLAB Live Script **`CompressorOptimization.mlx`**, developed as part of the **Turbomachinery course** in the 3rd year of Aerospace Engineering.  

The work focuses on the **preliminary design and optimization of an axial compressor stage**, using fundamental relations from thermodynamics, fluid dynamics, and turbomachinery design.  

---
## 🎯 Objectives  

- Evaluate compressor performance based on design inputs such as **mass flow rate, pressure ratio, and rotational speed**.  
- Apply **aerodynamic and thermodynamic constraints** (e.g., maximum relative Mach number, diffusion factor limits) to ensure feasible design.  
- Optimize compressor stage parameters to balance efficiency, stability, and performance.  

---

## 🧩 Methodology  

The MATLAB Live Script implements:  

1. **Thermodynamic State Calculations**  
   - Inlet conditions: stagnation temperature T₁, stagnation pressure P₁, and specific gas properties (R, γ, Cp).  
   - Outlet conditions computed using the **isentropic relation** for total temperature rise:  
     ```
     T₂ / T₁ = (P₂ / P₁)^((γ-1)/γ)
     ```  

2. **Velocity Triangle Relations**  
   - Blade speed U estimated from shaft speed and radius.  
   - Flow and relative Mach numbers checked against design constraints.  

3. **Compressor Constraints**  
   - **Relative Mach number constraint**:  
     ```
     M_rel,1 ≤ M_rel,max
     ```  
   - **Diffusion factor (DF) constraint**:  
     ```
     DF ≤ DF_max
     ```  

4. **Design Parameter Checks**  
   - Hub-to-tip ratio, solidity, and blade geometry feasibility.  
   - Aerodynamic stability margins considered.  

---

## 📂 File Description  

- **`CompressorOptimization.mlx`** – Main MATLAB Live Script containing code, explanations, and results.  
---

## 🛠️ Requirements  
- **MATLAB R2022a** or newer.  
- Toolboxes (depending on implementation):  
  - Optimization Toolbox (if optimization routines are used).  
  - Symbolic Math Toolbox (if symbolic derivations are included).  
---

## 📊 Expected Results  

- Compressor **inlet/outlet thermodynamic states**.  
- **Blade velocity and flow coefficients**.  
- Feasibility evaluation with respect to Mach number and diffusion factor limits.  
- Plots illustrating parameter trends and optimization results. 

---


# bladeless-wind-turbine-cfd
# Bladeless Wind Turbine — CFD Numerical Analysis
## CFD and Applications Module (7ENT2059) — University of Hertfordshire | 2025
### Group Project — CFD Simulation Lead: Rupeshwaran Paranthaman

## My Contribution
Responsible for all ANSYS Fluent simulations, computational 
domain setup, mesh generation, boundary condition 
configuration, solver settings, and results analysis. 
Group members contributed presentation formatting and narration.

## Project Overview
Comprehensive CFD analysis of external airflow around a 
bladeless wind turbine using ANSYS Fluent. The study 
investigated velocity distribution, pressure drop, wake 
formation, and turbine performance through numerical simulation.

## Tools Used
- ANSYS Fluent 2025 R2 — CFD solver and post-processing
- ANSYS Meshing — surface and volume mesh generation
- Watertight Geometry workflow — computational domain setup

## Computational Domain
| Parameter | Value |
|-----------|-------|
| Upstream length | 1,500 mm |
| Downstream length | 5,000 mm |
| Domain clearance | 1,000 mm |
| Inlet velocity (Group 10) | 44 m/s |
| Solver type | Double Precision 3D |
| Parallel processes | 5 |

## Methodology

### 1. Geometry & Domain Setup
Rectangular computational enclosure created using the 
Watertight Geometry workflow in ANSYS Fluent. Domain 
dimensions designed to ensure fully developed inlet flow 
upstream and complete wake capture downstream, with 
sufficient clearance to eliminate blockage effects.

### 2. Mesh Generation
- Surface mesh: 3mm face size with 1.2 growth rate
- Volume mesh: polyhedral mesh using global sizing
- Mesh quality validated through convergence checks
- Adaptive sizing based on curvature and proximity

### 3. Solver Settings
- Double Precision 3D solver for high-fidelity results
- 5 parallel meshing and solver processes
- k-ω turbulence model
- 1,000 iterations with convergence monitoring

### 4. Boundary Conditions
- Inlet: uniform velocity 44 m/s
- Outlet: pressure outlet (0 Pa reference)
- Walls: no-slip condition
- Ground: wall boundary

## Key Results

| Parameter | Value |
|-----------|-------|
| Inlet pressure | 15.805 Pa |
| Outlet pressure | 0 Pa (reference) |
| Pressure drop (ΔP) | 15.805 Pa |
| Mass flow rate (net) | 4.448062 × 10⁻⁵ kg/s |
| Convergence | Achieved — residuals stable |

## Key Findings
- Velocity streamlines confirmed stable and fully developed 
  inlet flow upstream of the turbine
- Low-velocity wake region identified downstream — 
  confirming momentum loss and flow separation
- Residuals for continuity, velocity components (x, y, z) 
  and turbulence variables (k and ω) decreased steadily 
  confirming numerical stability
- Pressure drop of 15.805 Pa extracted across the domain 
  representing total flow resistance
- Power calculation performed using P = τ × ω from 
  torque values extracted via ANSYS Fluent force reports
- Velocity magnitude contours revealed flow acceleration 
  around turbine and downstream wake recovery

## Results

### Computational Domain Setup
![Domain Setup](domain-setup.png)

### Surface Mesh Generation
![Surface Mesh](surface-mesh.png)

### Volume Mesh Generation  
![Volume Mesh](volume-mesh.png)

### Residual Convergence History
![Residual Convergence](residual-convergence.png)

### Velocity Streamlines
![Velocity Streamlines](velocity-streamlines.png)

### Velocity Magnitude Contours
![Velocity Contours](velocity-contours.png)

### Pressure Distribution
![Pressure Distribution](pressure-distribution.png)

### Power & Torque Calculation
![Power Calculation](power-calculation.png)

## Full Report
[Download Full Presentation Report](Bladeless-Wind-Turbine-CFD-Report.pdf)

## Skills Demonstrated
- External aerodynamic CFD simulation (ANSYS Fluent)
- Computational domain setup and boundary conditions
- Surface and volume mesh generation
- Turbulence modelling (k-ω)
- Convergence monitoring and validation
- Post-processing: velocity streamlines, pressure 
  contours, flux analysis
- Power and pressure drop extraction from CFD results
- Engineering analysis and result interpretation

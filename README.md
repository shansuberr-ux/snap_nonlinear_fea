# Snap-Fit Non-Linear FEA 

> **Ansys Mechanical · Non-Linear FEA · Plastic Design ·**

Non-linear finite element analysis of snap-fit features. The simulation captures large-deformation behavior during both insertion and removal — providing quantified snap-in force, removal force, and FOS data to drive design decisions on a real product.

---

## Project Overview

| Item | Detail |
|---|---|
| **Context** | Production snap-fit design |
| **Analysis Type** | Non-linear static structural (large deformation) |
| **Software** | Ansys Mechanical |
| **Geometry** | Cantilevered snap-fit wings for easy removal and assembly|
| **Iterations** | Multiple design versions simulated (V10+) |

---

## Key Results

| Parameter | Value |
|---|---|
| **Snap-in (insertion) force** | 38 N (3.8 kg) |
| **Snap-out (removal) force** | 30 N (3.0 kg) |
| **Max stress during insertion** | 57.2 MPa |
| **Material yield strength** | 65 MPa |
| **FOS at fillet** | 1.13 — flagged for redesign |
| **Recommended fix** | Increase fillet radius to 1.5mm or remove ribs |

---

## Why Non-Linear FEA?

Snap-fit hooks undergo large elastic deflections during assembly — routinely exceeding strains where linear assumptions break down. A linear model would misrepresent both the deflection and the force profile through the snap engagement. Non-linear analysis with large deformation enabled gives accurate force-displacement curves and realistic stress distributions at peak engagement.

---

## Gallery

| Snap Geometry — CAD Model | Deformation at 30N Removal |
|---|---|
| ![Model](https://github.com/shansuberr-ux/snap_nonlinear_fea/blob/main/pic.jpeg) | ![Deformation](https://github.com/shansuberr-ux/snap_nonlinear_fea/blob/main/wing%20evaluation2.jpeg) |

| Force-Displacement Curve & Stress Map |
|---|
| ![FEA results](https://github.com/shansuberr-ux/snap_nonlinear_fea/blob/main/snap%20resultant.jpeg) |

The force-displacement curve clearly shows the snap engagement peak at ~38N, followed by a drop as the snap clears — the classic non-linear snap-fit signature. Peak stress of 57.2 MPa occurs at the fillet, close to the 65 MPa yield strength (FOS 1.13), which drove the recommendation to increase fillet radius to 1.5mm.

---

## Simulation Workflow

1. Import snap-fit CAD, suppress non-critical features
2. Assign elastic-plastic material properties for the target polymer
3. Fixed support at chassis base; displacement-controlled loading on mating surface
4. Large deformation ON; substep convergence control
5. Extract force-displacement curve, von Mises stress, total deformation

---

## Skills Demonstrated

`Ansys Mechanical` `Non-Linear FEA` `Large Deformation Analysis` `Snap-Fit Design` `Plastic Part Design` `Stress Analysis` `Design Iteration` `Production Engineering`

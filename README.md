# Robust Fault Tolerant Controller for Quadrotors Using INDI

This repository contains the MATLAB/Simulink simulation model and the comprehensive undergraduate thesis report for the project titled **"ROBUST FAULT TOLERANT CONTROLLER FOR QUADROTORS USING INCREMENTAL NONLINEAR DYNAMIC INVERSION"**.

## Repository Contents

* **`INDI_QUAD_2021a.slx`**: The main Simulink model containing the nonlinear quadrotor simulation platform and the implemented controller.
* **`Magesvar_VR_UG_Project.pdf`**: The full project report detailing the mathematical modeling, Incremental Nonlinear Dynamic Inversion (INDI) control theory, fault modeling, and comprehensive simulation results.

---

## Key Features

* **INDI Control Law**: Utilizes Incremental Nonlinear Dynamic Inversion, a sensor-based nonlinear control approach that significantly reduces dependency on exact mathematical models, making the system highly robust against model uncertainties.
* **Cascaded Two-Loop Structure**: Implements a cascaded linear controller design for the outer loop to manage position (x, y), altitude (z), and yaw effectively.
* **Loss of Effectiveness (LOE) Fault Modeling**: Incorporates an LOE fault model to simulate partial actuator failures by representing the fault as a loss in control input rather than a physical hardware break.
* **Proven Fault Tolerance**: Demonstrates through simulations that the quadrotor maintains stability and tracking performance with up to a 65% loss of effectiveness in the actuators.

---

## Simulation Details & Parameters

* **Quadrotor Base Model**: The dynamic model is based on the UAVision UXSpyro quadrotor.
* **Motor Specifications**: Modeled after the T-motor P60 340 KV paired with a 22x6.6 CF propeller.
* **Sampling Time**: The INDI controller relies on input dynamics being faster than state dynamics. The simulation uses a high sampling frequency of 1000 Hz (a sampling time of 0.001 seconds) for optimal tracking.
* **Testing Scenarios**: The model is evaluated using continuous helical trajectories and step-response waypoints.

---

## Authors & Acknowledgments

This project was developed by undergraduate researchers at the Amrita School of Engineering, Coimbatore, Department of Aerospace Engineering:

* **Magesvar V R**
* **Ashwin B**
* **Kunapareddy Lokesh Sai**
* **Shri Vathsan**

**Project Guide:** Dr. Jinraj V Pushpangathan

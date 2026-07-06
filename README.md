# [cite_start]Robust Fault Tolerant Controller for Quadrotors Using INDI [cite: 662]

[cite_start]This repository contains the MATLAB/Simulink simulation model and the comprehensive undergraduate thesis report for the project titled **"ROBUST FAULT TOLERANT CONTROLLER FOR QUADROTORS USING INCREMENTAL NONLINEAR DYNAMIC INVERSION"**[cite: 662].

[cite_start]The primary objective of this project is to stabilize a quadrotor in the event of actuator or propeller faults (such as a lock-in place, float, or hard-over hardware failures) and improve tracking performance so the quadrotor can land safely[cite: 859, 861, 1070, 1071].

## Repository Contents

* [cite_start]**`INDI_QUAD_2021a.slx`**: The main Simulink model containing the nonlinear quadrotor simulation platform and the implemented controller[cite: 650].
* [cite_start]**`Magesvar_VR_UG_Project.pdf`**: The full project report detailing the mathematical modeling, Incremental Nonlinear Dynamic Inversion (INDI) control theory, fault modeling, and comprehensive simulation results[cite: 651].

---

## Key Features

* **INDI Control Law**: Utilizes Incremental Nonlinear Dynamic Inversion, a sensor-based nonlinear control approach that significantly reduces dependency on exact mathematical models, making the system highly robust against model uncertainties[cite: 960, 974].
* [cite_start]**Cascaded Two-Loop Structure**: Implements a cascaded linear controller design for the outer loop to manage position (x, y), altitude (z), and yaw effectively[cite: 897, 1125, 1133].
* [cite_start]**Loss of Effectiveness (LOE) Fault Modeling**: Incorporates an LOE fault model to simulate partial actuator failures by representing the fault as a loss in control input rather than a physical hardware break[cite: 1074].
* **Proven Fault Tolerance**: Demonstrates through simulations that the quadrotor maintains stability and tracking performance with up to a 65% loss of effectiveness in the actuators[cite: 1176, 1177].

---

## Simulation Details & Parameters

* [cite_start]**Quadrotor Base Model**: The dynamic model is based on the UAVision UXSpyro quadrotor[cite: 996].
* [cite_start]**Motor Specifications**: Modeled after the T-motor P60 340 KV paired with a 22x6.6 CF propeller[cite: 1056, 1057].
* **Sampling Time**: The INDI controller relies on input dynamics being faster than state dynamics[cite: 965, 1152]. The simulation uses a high sampling frequency of 1000 Hz (a sampling time of 0.001 seconds) for optimal tracking[cite: 1159].
* [cite_start]**Testing Scenarios**: The model is evaluated using continuous helical trajectories and step-response waypoints[cite: 1147, 1208].

---

## Authors & Acknowledgments

[cite_start]This project was developed by undergraduate researchers at the Amrita School of Engineering, Coimbatore, Department of Aerospace Engineering[cite: 662, 664]:

* **Magesvar V R** [cite: 662]
* [cite_start]**Ashwin B** [cite: 662]
* [cite_start]**Kunapareddy Lokesh Sai** [cite: 662]
* **Shri Vathsan** [cite: 662]

**Project Guide:** Dr. Jinraj V Pushpangathan [cite: 662]

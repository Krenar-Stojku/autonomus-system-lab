# Scenario : Human Driver Override

##  Overview

This scenario addresses a situation where a human driver manually overrides the autonomous control of a truck within an active platoon. Manual override may be initiated due to unforeseen situations such as navigation adjustments, hardware malfunctions, or emergency responses. The platooning system must be designed to handle such overrides gracefully and safely, ensuring that the platoon's overall behavior remains stable and collision-free.

---

##  Objective

The main objective is to ensure that the autonomous system detects a manual override in real time, initiates safe detachment of the truck, and reconfigures the rest of the platoon automatically. The scenario focuses on:

- Real-time detection of manual input (e.g., steering, braking)
- Notification and coordination between vehicles
- Safe disengagement of the overridden truck
- Reconfiguration of platoon roles and spacing

---

##  Real-World Relevance

In real-world highway automation, human intervention remains a critical fallback option. Ensuring that platooning systems are robust to such transitions is essential for:

- Road safety and liability compliance
- User trust and system transparency
- Interoperability with semi-autonomous vehicles

---

##  System Behavior Summary

1. *Override Detection:*  
   The onboard system of the truck continuously monitors for manual input. If a steering wheel, brake, or accelerator input is detected, the override mode is triggered within 100 ms.

2. *Notification:*  
   The overridden truck sends a real-time message to the platoon leader and following vehicles to announce its transition to manual mode.

3. *Platoon Adjustment:*  
   Other trucks receive and acknowledge the signal, then automatically adjust spacing and reassign roles (e.g., new leader if needed).

4. *Safe Disengagement:*  
   The manually controlled truck decelerates or changes lanes based on safety logic and exits the platoon.

5. *Stabilization:*  
   The remaining trucks maintain a safe, coordinated platoon configuration without the detached vehicle.

---

##  Why This Scenario Matters

- It tests *system robustness* in the presence of human unpredictability.
- It reflects realistic *mixed-control environments* (autonomous + manual).
- It supports *fail-safe operation* when autonomy is interrupted.
- It demonstrates the system’s *adaptability and resilience*.

---
<div align="center">
  
  <img src="banner.png" alt="OURANOS Logo" width="600">

  <h3>Mission-Driven Generative Aircraft Engineering</h3>

  <p>
    <strong>
      <code>MISSION</code> → 
      <code>ARCHITECTURE</code> → 
      <code>ENGINEERING</code> → 
      <code>PACKAGING</code> → 
      <code>VALIDATION</code> → 
      <code>CAD</code>
    </strong>
  </p>

  <p>
    <img src="https://img.shields.io/badge/STATUS-ACTIVE%20R%26D-111827?style=for-the-badge">
    <img src="https://img.shields.io/badge/DOMAIN-AEROSPACE-0F172A?style=for-the-badge">
    <img src="https://img.shields.io/badge/ENGINEERING-PARAMETRIC-1E293B?style=for-the-badge">
    <img src="https://img.shields.io/badge/PIPELINE-SYSTEMS%20FIRST-000000?style=for-the-badge">
  </p>
</div>

<br/>

## 🪐 OURANOS (Οὐρανός)

In Greek mythology, Ouranos is the primordial personification of the sky. 

The name represents the idea of an engineering system that operates across the entire aircraft design space — from the first mission requirement to the complete aircraft system. The project takes its name from the Greek concept of the **sky itself** rather than from a specific aircraft.

> **One mission. Many possible aircraft.**

---

<div align="center">
  <img src="assets/hero-uav.jpg" width="95%" style="border-radius: 8px;">
</div>

<br/>

## 🛠 A Different Approach to Aircraft Design

Most aircraft generators focus primarily on external geometry. OURANOS is designed around a fundamentally different principle:

> **Do not generate an aircraft shell. Generate an aircraft system.**

A design is not considered complete when the exterior looks correct. It is complete when the following sub-systems all agree with one another without physical or dynamic conflict:

* **Airframe & Structure**
* **Control Surfaces & Servos**
* **Propulsion & Battery**
* **Avionics, Sensors & Cameras**
* **Antennas & Landing Gear**
* **Internal Packaging & Routing**

---

## 🏗 SYSTEM ARCHITECTURE

<div align="center">
  <img src="assets/ouranos-system-diagram.png" width="90%">
</div>

```text
MISSION REQUIREMENTS
        │
        ▼
ARCHITECTURE SYNTHESIS
        │
        ▼
AIRCRAFT SIZING
        │
        ▼
PARAMETRIC GEOMETRY
        │
        ├──────────────────────────┐
        ▼                          ▼
PHYSICAL COMPONENTS        INTERNAL STRUCTURE
        │                          │
        └────────────┬─────────────┘
                     ▼
             INTERNAL PACKAGING
                     │
                     ▼
           ENGINEERING VALIDATION
                     │
                     ▼
             MDO OPTIMIZATION
                     │
                     ▼
                CAD ASSEMBLY
🌌 DESIGN SPACEOURANOS is designed to explore fundamentally different aircraft architectures.Not: ONE AIRCRAFT × 50 COSMETIC VARIATIONSInstead: MULTIPLE ARCHITECTURES × MULTIPLE GEOMETRIES × PROPULSION LAYOUTS × PAYLOADSPossible Configurations:High-wing, low-wing, shoulder-wingFlying-wing, twin-boom, V-tail, T-tailPusher, tractor, twin-motor, motor-gliderModular payload and experimental architectures⚙️ PARAMETRIC DEPENDENCY GRAPHThe central concept of OURANOS is the dependency graph. Changing one parameter propagates physically and aerodynamically through the entire aircraft.Dependency Flow ExamplesPropulsion: Larger Motor → Motor Mount → ESC Requirement → Cooling Needs → Mass Shift → Center of Gravity → Battery Resizing → Internal Packaging → Structure UpdateControl Surface: Larger Flap → Higher Aero Load → Larger Servo Req. → Expanded Servo Bay → Reinforced Linkage → Wing Structure UpdatePayload: Second Camera → Added Mass → CG Shift → Mounting Structure → Internal Volume Deduction → Cable Routing Conflict📦 INTERNAL PACKAGING & VALIDATIONThe aircraft is never treated as an empty shell. Internal space is strictly managed for batteries, flight controllers, GPS, airspeed sensors, ESCs, telemetry, antennas, servos, and structural elements.Automated Engineering ChecksEvery generated configuration passes through a rigorous multi-physics engineering filter. The objective is to identify exactly why a design is valid or invalid.ParameterValidation MetricStatus ExampleMass PropertiesCG Range & Inertia🟢 PASSAerodynamicsWing Loading & Stall Speed🟢 PASSPropulsionStatic Thrust & Motor Fit🟢 PASSPackagingBattery Volume & Servo Clearance🔴 ERRORSensorsAirspeed Placement & Camera Fit🟢 PASSRF SystemsAntenna Clearance (Ground)🟢 PASSManufacturingStructural Interfaces🟡 WARNING🖥 FROM CONCEPT TO CADThe long-term objective is not an attractive render. It is a structured, parametrically connected aircraft assembly ready for real-world engineering.PlaintextCONCEPT → ENGINEERING MODEL → PARAMETRIC GEOMETRY → COMPONENT PACKAGING → VALIDATION → CAD ASSEMBLY
📑 PROJECT STATUSOURANOS is an independent research and engineering project.The project explores mission-driven generative aircraft design, parametric engineering, system-level configuration, and CAD-oriented development.This public repository is intended to document the research direction, engineering concepts, visual demonstrations, and development progress. Core implementation, proprietary algorithms, internal engineering models, and private component databases are not distributed publicly.

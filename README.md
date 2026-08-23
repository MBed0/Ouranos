# OURANOS

### Mission-Driven Generative Aircraft Engineering

<p align="center">
  <img src="banner.png" width="%70">
</p>

<p align="center">
  <strong>MISSION → ARCHITECTURE → ENGINEERING → PACKAGING → VALIDATION → CAD</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/STATUS-RESEARCH%20%26%20DEVELOPMENT-111827?style=for-the-badge">
  <img src="https://img.shields.io/badge/AEROSPACE-ENGINEERING-0F172A?style=for-the-badge">
  <img src="https://img.shields.io/badge/PARAMETRIC-DESIGN-1E293B?style=for-the-badge">
</p>

---

## OURANOS

**Ouranos — Οὐρανός**

In Greek mythology, Ouranos is the primordial personification of the sky.

The name represents the idea of an engineering system that operates across the entire aircraft design space — from the first mission requirement to the complete aircraft system.

The project takes its name from the Greek concept of the **sky itself** rather than from a specific aircraft.

> **One mission.
> Many possible aircraft.**

---

<p align="center">
  <img src="assets/hero-uav.jpg" width="92%">
</p>

## A Different Approach to Aircraft Design

Most aircraft generators focus primarily on external geometry.

OURANOS is designed around a different principle:

> **Do not generate an aircraft shell. Generate an aircraft system.**

A design is not considered complete when the exterior looks correct.

It is complete when:

```text
AIRFRAME
+
CONTROL SURFACES
+
SERVOS
+
PROPULSION
+
BATTERY
+
AVIONICS
+
SENSORS
+
CAMERAS
+
ANTENNAS
+
STRUCTURE
+
LANDING GEAR
+
INTERNAL PACKAGING
```

all agree with one another.

---

## SYSTEM ARCHITECTURE

<p align="center">
  <img src="assets/ouranos-system-diagram.png" width="88%">
</p>

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
        ├───────────────┐
        ▼               ▼
  COMPONENTS       STRUCTURE
        │               │
        └───────┬───────┘
                ▼
        INTERNAL PACKAGING
                │
                ▼
        ENGINEERING VALIDATION
                │
                ▼
            OPTIMIZATION
                │
                ▼
           CAD ASSEMBLY
```

---

# DESIGN SPACE

<p align="center">
  <img src="assets/architecture-exploration.png" width="94%">
</p>

OURANOS is designed to explore fundamentally different aircraft architectures.

Not:

```text
ONE AIRCRAFT × 50 COSMETIC VARIATIONS
```

Instead:

```text
MULTIPLE ARCHITECTURES
        ×
MULTIPLE GEOMETRIES
        ×
MULTIPLE PROPULSION LAYOUTS
        ×
MULTIPLE PAYLOAD CONFIGURATIONS
```

Possible configurations include high-wing, low-wing, shoulder-wing, flying-wing, twin-boom, V-tail, T-tail, pusher, tractor, twin-motor, motor-glider, modular payload and experimental architectures.

---

# THE AIRCRAFT IS A SYSTEM

<p align="center">
  <img src="assets/exploded-aircraft.png" width="90%">
</p>

Every major subsystem can exist as a real engineering component.

```text
AIRCRAFT
│
├── FUSELAGE
│
├── LEFT WING
│   ├── FLAP
│   ├── AILERON
│   ├── SERVO BAY
│   └── STRUCTURE
│
├── RIGHT WING
│   ├── FLAP
│   ├── AILERON
│   ├── SERVO BAY
│   └── STRUCTURE
│
├── TAIL
│
├── PROPULSION
│
├── BATTERY
│
├── AVIONICS
│
├── CAMERAS
│
├── AIRSPEED SYSTEM
│
├── ANTENNAS
│
└── LANDING GEAR
```

---

# PARAMETRIC DEPENDENCY GRAPH

<p align="center">
  <img src="assets/dependency-graph.png" width="86%">
</p>

The central concept of OURANOS is the dependency graph.

Changing one parameter can propagate through the aircraft.

### Example — Propulsion

```text
LARGER MOTOR
      ↓
MOTOR MOUNT
      ↓
ESC REQUIREMENT
      ↓
COOLING
      ↓
MASS
      ↓
CENTER OF GRAVITY
      ↓
BATTERY
      ↓
INTERNAL PACKAGING
      ↓
STRUCTURE
```

### Example — Control Surface

```text
LARGER FLAP
      ↓
AERODYNAMIC LOAD
      ↓
SERVO REQUIREMENT
      ↓
SERVO BAY
      ↓
LINKAGE
      ↓
WING STRUCTURE
```

### Example — Camera

```text
SECOND CAMERA
      ↓
MASS
      ↓
CG
      ↓
MOUNTING STRUCTURE
      ↓
INTERNAL VOLUME
      ↓
CABLE ROUTING
```

---

# CONTROL SURFACES

<p align="center">
  <img src="assets/control-surface-detail.png" width="82%">
</p>

Control surfaces are treated as independent physical components.

```text
LEFT FLAP
 ├── Geometry
 ├── Hinge
 ├── Control Horn
 ├── Linkage
 ├── Servo
 └── Servo Bay

RIGHT FLAP
 ├── Geometry
 ├── Hinge
 ├── Control Horn
 ├── Linkage
 ├── Servo
 └── Servo Bay
```

The same approach applies to ailerons, elevator, rudder, elevons, ruddervators and other architecture-dependent control systems.

---

# INTERNAL PACKAGING

<p align="center">
  <img src="assets/internal-packaging.jpg" width="90%">
</p>

The aircraft is not treated as an empty shell.

The internal system can contain:

```text
CAMERA BAY
PAYLOAD BAY
BATTERY
FLIGHT CONTROLLER
GPS
AIRSPEED SENSOR
ESC
RECEIVER
TELEMETRY
ANTENNAS
SERVOS
STRUCTURE
```

Packaging checks can identify:

```text
COMPONENT COLLISION
INSUFFICIENT VOLUME
INACCESSIBLE COMPONENT
CABLE ROUTING CONFLICT
SERVO INTERFERENCE
STRUCTURAL INTERFERENCE
CG PROBLEM
```

---

# ENGINEERING VIEW

<p align="center">
  <img src="assets/gui-preview.png" width="96%">
</p>

The intended interface is closer to an engineering workstation than a conventional 3D configurator.

```text
MISSION
ARCHITECTURE
GEOMETRY
CONTROL SURFACES
PROPULSION
BATTERY
AVIONICS
SENSORS
CAMERAS
ANTENNAS
LANDING GEAR
STRUCTURE
PACKAGING
AERODYNAMICS
MASS & CG
MANUFACTURING
OPTIMIZATION
CAD
REPORT
```

The viewport can independently reveal:

```text
AIRFRAME
STRUCTURE
SERVOS
CONTROL SURFACES
MOTOR
BATTERY
ELECTRONICS
CAMERAS
SENSORS
ANTENNAS
LANDING GEAR
```

---

# ENGINEERING VALIDATION

<p align="center">
  <img src="assets/validation-dashboard.png" width="88%">
</p>

Every generated configuration should pass through engineering checks.

```text
CG                         PASS
WING LOADING               PASS
STALL SPEED                PASS
PROPULSION                 PASS
BATTERY VOLUME             WARNING
MOTOR FIT                  PASS
ESC FIT                    PASS
SERVO PACKAGING            ERROR
CAMERA FIT                 PASS
AIRSPEED PLACEMENT         PASS
ANTENNA CLEARANCE          PASS
LANDING GEAR               PASS
STRUCTURAL INTERFACES      PASS
MANUFACTURABILITY          WARNING
```

The objective is not to make every design valid.

The objective is to **identify why a design is valid or invalid.**

---

# DESIGN EXPLORATION

<p align="center">
  <img src="assets/candidate-grid.png" width="94%">
</p>

A mission can produce a design space rather than a single answer.

```text
MISSION
   ↓
DESIGN SPACE
   ↓
CANDIDATE GENERATION
   ↓
ENGINEERING FILTER
   ↓
VALIDATION
   ↓
RANKING
   ↓
DESIGN 01 ... DESIGN 50
```

Each candidate can have a different:

* Architecture
* Wing geometry
* Tail configuration
* Propulsion arrangement
* Payload layout
* Camera configuration
* Landing gear
* Battery placement
* Avionics placement
* Internal packaging

---

# FROM CONCEPT TO CAD

<p align="center">
  <img src="assets/cad-assembly.jpg" width="90%">
</p>

The long-term objective is not an attractive render.

It is a structured, parametrically connected aircraft assembly.

```text
CONCEPT
   ↓
ENGINEERING MODEL
   ↓
PARAMETRIC GEOMETRY
   ↓
COMPONENT PACKAGING
   ↓
VALIDATION
   ↓
ASSEMBLY
   ↓
CAD
```

---

# PROJECT STATUS

**OURANOS is an independent research and engineering project.**

The project explores mission-driven generative aircraft design, parametric engineering, system-level configuration and CAD-oriented development.

The public repository is intended to document the research direction, engineering concepts, visual demonstrations and development progress.

Core implementation, proprietary algorithms, internal engineering models and private component databases are not distributed publicly.

---

## DESIGN PRINCIPLE

> **The aircraft is not the model.
> The aircraft is the system behind the model.**

<p align="center">

### OURANOS

**Mission → Engineering → Aircraft**

</p>

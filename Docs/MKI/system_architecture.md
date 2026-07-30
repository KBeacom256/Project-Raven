                      PROJECT RAVEN MKI
                    SYSTEM ARCHITECTURE

                    ┌──────────────────┐
                    │     Operator     │
                    │──────────────────│
                    │ Radio Controller │
                    │ Mission Planner  │
                    │ Walksnail Goggles│
                    └────────┬─────────┘
                             │
           ┌─────────────────┼─────────────────┐
           │                 │                 │
        ELRS RC         SiK Telemetry     Walksnail Video
           │                 │                 │
           ▼                 ▼                 ▼

┌──────────────────────────────────────────────────────────┐
│                  PROJECT RAVEN MKI UAV                   │
│                                                          │
│                 Flight Control System                    │
│      ┌─────────────────────────────────────────┐         │
│      │        Matek H743 Slim V3               │         │
│      │-----------------------------------------│         │
│      │ ArduPilot                               │         │
│      │ Sensor Fusion                           │         │
│      │ Navigation                              │         │
│      │ Flight Stabilization                    │         │
│      └─────────────────────────────────────────┘         │
│          ▲        ▲        ▲         ▲        ▲          │
│          │        │        │         │        │          │
│      Here4 GPS  RP3 ELRS  SiK     Walksnail  PM02        │
│       (UART)     (CRSF)  Radio     VTX      Power Module │
│                                                          │
│               Motor Control System                       │
│                                                          │
│          PWM / DShot Signals                             │
│                    │                                     │
│                    ▼                                     │
│            SEQURE 4-in-1 ESC                             │
│                    │                                     │
│      ┌──────┬──────┼──────┬──────┐                       │
│      ▼      ▼      ▼      ▼      │                       │
│   Motor1 Motor2 Motor3 Motor4    │                       │
│                                                          │
│                Power System                              │
│                                                          │
│ Battery (4S)                                             │
│      │                                                   │
│     XT60                                                 │
│      │                                                   │
│    PM02                                                  │
│      │                                                   │
│      ├──────────────► Flight Controller                  │
│      └──────────────► ESC                                │
│                                                          │
└──────────────────────────────────────────────────────────┘

-------------------------------
1. AIRFRAME
* Components
- Tony 5 carbon frame
- 3D printed TPU mounts
- Battery holder
- Landing gear
- Camera cage
--------------------------------
2. POWER SYSTEM
* Components:
- CNHL 4S battery
- XT60 connectors
- PM02 V3
- SEQURE ESC
- Wiring harness
* Outputs:
- Flight Controller
- ESC
- Camera/VTX
---------------------------------
3. FLIGHT CONTROL SYSTEM
* Components:
- Matek H743 Slim V3
- ArduPilot
- Here4 GPS
- RP3 ELRS receiver
- Sik Telemetry radio
* Responsibilities:
- Stabilization
- Navigation
- Waypoint missions
- Sensor fusion
- Motor mixing
- Flight logging
----------------------------------
4. PROPULSION
* Components:
- 4 x Motors
- 4 x propellers
- ESC
* Responsibilities:
- Hover
- Climb
- Pitch
- Roll
- Yaw
-----------------------------------
5. FPV SYSTEM
* Components:
- Walksnail Moonlight
- Walksnail Antenna
- Walksnail Goggles
* Responsibilities:
- Live HD video
- DVR recording
- Low-latency control
--------------------------------------------------------------------------------

Pilot Inputs
      │
      ▼
ELRS Receiver
      │
      ▼
Matek H743
      │
      ▼
Motor Commands
      │
      ▼
ESC
      │
      ▼
Motors

------------------------------------------------------------------------------

GPS
 │
 ▼
Flight Controller
 │
 ▼
Autonomous Navigation

-----------------------------------------------------------------------------

Camera
 │
 ▼
Walksnail VTX
 │
 ▼
Walksnail Goggles

-----------------------------------------------------------------------------

Flight Controller
 │
 ▼
SiK Radio
 │
 ▼
Mission Planner




------------Project Raven Family-----------------------

MKI
│
├── Flight software development
├── Hardware validation
├── Sensor testing
└── Pilot training

        │ Lessons learned
        ▼

MKII
├── Heavy-lift platform
├── Dual-battery system
├── Payload integration
└── Advanced autonomous missions
























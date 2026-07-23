What systems are required and their purpose:
                 Ground Control Station
              (Mission Planner / QGC)
                        │
         ┌──────────────┴──────────────┐
         │                             │
    MAVLink Telemetry             ELRS Control
         │                             │
         └──────────────┬──────────────┘
                        │
             ┌─────────────────────┐
             │      Raven Mk I     │
             │ Flight Controller   │
             │ GPS / Compass / IMU │
             │ Power System         │
             │ Analog Camera        │
             └─────────────────────┘

                        │
                Proven technologies
                        ▼

             ┌─────────────────────┐
             │      Raven Mk II    │
             │ Flight Controller   │
             │ GPS / Compass / IMU │
             │ HD Video System      │
             │ Companion Computer   │
             │ Payload Interfaces   │
             └─────────────────────┘



- Battery               == Provide stable power at a constant rate
- Power module          == Protect electronics and saftey
- Flight controller     == Autonomous navigation flight logging and stabilization
--- GPS                 == Return to launch waypoint navigation and position holding
--- ELRS Reciever       == Pilot control manuel override and flight mode selection
--- Telementary Radio   == aircraft monitor mission upload and log download
--- Camera              == navigation
--- ESCs                == Maintain stable distributuion
----- Motors            == Maintain stable flight and resist wind disturbances
------- Propellers      == Ensure balance stability and lifting power
- Frame                 == Structual support and protect electronics absorb crash loads

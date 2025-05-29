# Timing Behavior – Scenario 11: Human Driver Override

| Event                        | Time Constraint  | Description                                       |
|------------------------------|------------------|---------------------------------------------------|
| Detect driver input          | ≤ 100 ms         | Input (steering/brake) triggers override detection|
| Send override signal         | ≤ 250 ms         | Message sent to platoon leader and other trucks   |
| Acknowledge override         | ≤ 500 ms         | Other trucks acknowledge the override             |
| Start reconfiguration        | ≤ 1 sec          | Platoon adjusts gaps and roles                    |
| Reconfiguration complete     | ≤ 3 sec          | System returns to stable platoon configuration    |
| Safety margin maintained     | Continuous       | Distance ≥ 30m is preserved during the process    |
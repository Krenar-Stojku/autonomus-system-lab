# Requirements – Human Driver Override

## Detection Requirements
- The truck system must detect steering, throttle, or brake input from the human driver within 100 ms.
- Manual control mode must be confirmed before any disengagement.

## Notification Requirements
- The overridden truck must send an override event to the platoon leader and following trucks within 250 ms.
- All trucks must acknowledge receipt of this signal.

## Behavioral Requirements
- The overridden truck must initiate a safe deceleration or lane change to exit the platoon.
- Other trucks must adjust their inter-vehicle gaps accordingly.
- Role reconfiguration (e.g., new leader if necessary) must be triggered automatically.

## Safety Requirements
- A minimum safe distance (≥ 30 meters) must be ensured during the override and detachment.
- The system must prevent collisions even in the event of delayed communication.

## Fallback Requirements
- If the override signal is not received by any truck, the platoon must assume the truck is exiting and reconfigure preemptively.
- All such events must be logged and reported to the central fleet management system.
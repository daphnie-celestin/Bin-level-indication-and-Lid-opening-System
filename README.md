# Bin-level-indication-and-Lid-opening-System
This system automatically indicates the fill level of the bin and opens the lid when needed.

1. System Setup
- Mount IR sensor inside the bin to monitor trash level.
- Mount PIR sensor on the outer body of the bin to detect motion.
- Connect a servo motor to the bin lid for automated opening.

2. Lid Opening Logic
- PIR sensor detects human presence.
- If a person is within range, Arduino sends a signal to servo motor.
- Servo motor rotates to open the lid (90°).
- After a delay (e.g., 5 seconds), the lid closes again (returns to 0°).

3. Bin Fill Level Indication
- IR sensor continuously measures the distance from the top of the bin to the waste.
- If the value is less than a threshold (e.g., 40), bin is considered full.
- Arduino sends a message (e.g., “Bin is full”) via Serial Monitor.

Demonstrates a simple, low-cost, and efficient Embedded system for modern waste management.

# Week 2: Logic, Circuits & Animatronics

**Instructor:** Alvaro

---

## Learning Objectives

- Understand basic circuit concepts: voltage, current, LEDs, sensors
- Build and simulate circuits in Tinkercad
- Wire a physical circuit using an Arduino and breadboard
- Program a servo motor to control a pre-built animatronic eye

---

## Session 1 (Day 1): Circuit Logic & Virtual Prototyping

### Key components
| Part | Role |
|------|------|
| **Arduino** | Programmable microcontroller — the brain |
| **Breadboard** | Prototyping board for connecting components without soldering |
| **LED** | Lights up when current flows through it |
| **Resistor** | Limits current to protect components |
| **Sensor** | Reads input from the physical world |

### Tinkercad Circuits (browser simulation)
1. Go to [tinkercad.com](https://www.tinkercad.com) — create a free account
2. Click "Circuits" > "Create new Circuit"
3. Build a virtual LED blink circuit with an Arduino

**In-class activity:** Build a virtual circuit in Tinkercad, then replicate it on a real breadboard.

---

## Session 2 (Day 2): Animatronics & Servo Control

A **servo motor** rotates to a specific angle (0-180 degrees) — the basis of animatronics.

**In-class activity: Animatronic Eye**
1. Receive a pre-3D-printed animatronic eye assembly
2. Attach a servo motor
3. Connect to Arduino and upload code to make the eye move

**Sample code:**
```cpp
#include <Servo.h>
Servo eyeServo;
void setup() { eyeServo.attach(9); }
void loop() {
  eyeServo.write(45);  delay(1000);  // look left
  eyeServo.write(90);  delay(1000);  // center
  eyeServo.write(135); delay(1000);  // look right
}
```

---

## Homework

Visit the **Robotics Lab** for a Sense Hat & Raspberry Pi orientation. Check Canvas for schedule and room.

---

## Resources

- [Tinkercad Circuits](https://www.tinkercad.com/circuits)
- [Arduino IDE download](https://www.arduino.cc/en/software)
- [Arduino Servo tutorial](https://www.arduino.cc/en/Tutorial/LibraryExamples/Sweep)

## Project & Assignment

See [ASSIGNMENT.md](ASSIGNMENT.md) for full requirements and grading.

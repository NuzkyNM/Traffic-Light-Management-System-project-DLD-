# Traffic Light Management System project (DLD)
A hardware-based traffic light control system for a four-way intersection using a 555 timer and 4017 Decade Counter IC. Fully timed LED sequencing with no microcontroller or sensors involved.

## Project Overview

This system manages traffic at a four-way intersection using only hardware logic. It uses a 4017 decade counter IC to control four sets of traffic lights, each consisting of Red, Yellow, and Green LEDs. A timer circuit (typically 555 Timer IC or similar) is used to trigger the 4017 to cycle through traffic signals at fixed intervals.

## Features

- Four sets of traffic lights (each with Red, Yellow, Green LEDs)
- Timed control using 4017 IC
- No programming or microcontroller required
- Includes an LED for countdown indication
- Fully hardware-based and cost-effective

## Components Used

- 4017 Decade Counter IC  
- 555 Timer IC (or alternative clock source)  
- LEDs (4 sets of Red, Yellow, Green)  
- Resistors (various values)  
- Capacitors (for timer circuit)  
- Breadboard or PCB  
- Connecting wires  
- Power supply (5V or 9V depending on design)

## Circuit Description

The timer circuit generates clock pulses at fixed intervals. These pulses drive the 4017 IC, which sequentially activates its output pins. Each output controls one traffic light set (Red → Green → Yellow). After completing one full cycle, the process repeats.

An extra LED is used to indicate a basic countdown for time awareness.

## How It Works

1. The timer sends clock pulses to the 4017 IC.
2. The IC sequentially activates its output pins.
3. Each output is wired to a traffic light set.
4. The LEDs change in a timed sequence, simulating real-world traffic lights.

## Limitations

- No vehicle detection (IR or ultrasonic sensors not used)
- Fixed timing, no adaptive control
- No pedestrian or emergency signal support

## Future Improvements (Optional)

- Add microcontroller-based control for dynamic timing
- Use IR sensors for vehicle detection
- Add pedestrian buttons and buzzers
- LCD or 7-segment display for countdown timer

## License

This project is open-source under the MIT License.

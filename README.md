# Analog Circuit Design Projects

This repository contains documentation and simulation files for analog circuit design projects, focusing on practical applications and mixed-signal systems.

## Project Overview

### 1. Alarm for Sleep Prevention

**Objective**: 
Design a tilt sensor-based alarm system to detect signs of drowsiness and prevent sleep during critical tasks.

**Key Components**:
- Tilt Sensor
- 555 Timer IC (Monostable Multivibrator Configuration)
- Buzzer
- LM7805 Voltage Regulator

**Methodology**:
- The tilt sensor detects user movement and triggers a monostable pulse using the 555 Timer IC
- If no tilt/movement is detected, a buzzer sounds an alarm

**Simulation Tools**:
- Tinkercad Electronics Simulator

**Results**:
- Successfully demonstrated real-time detection of drowsiness through tilt sensing and alarm activation

### 2. Design of a 6-bit Fully Differential Current-Steering DAC

**Objective**: 
Design and simulate a 6-bit fully differential current-steering DAC suitable for mixed-signal applications.

**Key Components**:
- PMOS Current Sources
- Row and Column Decoder Logic
- 180nm CMOS Technology Models

**Methodology**:
- Designed a schematic of the DAC in LTSpice focusing on minimizing static and dynamic non-linearities
- Performed transient and DC analyses to characterize DAC performance metrics
- Optimized transistor sizing to improve matching and current source stability

**Simulation Tools**:
- LTSpice

**Results**:
- Achieved low static non-linearity with **INL and DNL < 0.5 LSB**
- Estimated power consumption below **1 mW** at nominal conditions
- Analyzed skew and glitch energy from transient outputs

## Repository Structure

```
├── Sleep-Prevention-Alarm/
│   ├── report with simulations/
├── 6bit-Current-Steering-DAC/
│   ├── report with simulations/
└── README.md
```

## Getting Started

### Prerequisites
- Tinkercad account (for Sleep Prevention Alarm simulation)
- LTSpice (for DAC simulations)
- Basic understanding of analog electronics and circuit design

### Running Simulations

#### Sleep Prevention Alarm
1. Open the Tinkercad simulation file in your browser
2. Adjust the tilt sensor positioning to observe the alarm behavior
3. Modify timing parameters as needed for different sensitivity levels

#### 6-bit Current-Steering DAC
1. Open the .asc schematic files in LTSpice
2. Run transient analysis to observe DAC output behavior
3. Modify component values to experiment with performance tradeoffs

## Future Work

- Implement PCB design for the Sleep Prevention Alarm
- Expand the DAC design to higher resolution (8-bit)
- Analyze temperature effects on both circuit designs
- Create physical prototypes and compare with simulation results

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

For questions or collaboration opportunities, please open an issue in this repository.

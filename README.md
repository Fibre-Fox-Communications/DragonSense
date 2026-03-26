# 🐉 DragonSense
**Reptile Enclosure Environmental Monitoring & Control System**

<img width="100%" align="center" src ="https://github.com/Fibre-Fox-Communications/DragonSense/blob/main/Repo_Images/DragonSenseBanner.png?raw=true" >

## Overview
**DragonSense** is a modular environmental monitoring and control system designed for reptile enclosures. Built around the **RP2040 microcontroller**, it provides precise control over heating, lighting, airflow, and environmental conditions to help maintain a stable and healthy habitat.

The system combines **real-time sensing**, **automated control**, and a **web-based interface**, with future expansion planned for platforms such as **Home Assistant**.

---

## Features

### Environmental Monitoring
- Temperature sensing
- Humidity monitoring
- UV sensing
- Real-time telemetry and status reporting

### Environmental Control
- Relay-controlled outputs for:
  - UV lighting
  - Basking lamps
- PWM or variable control for:
  - LED lighting
  - Cooling and circulation fans

### Web Interface
- Embedded web dashboard for:
  - Live sensor readings
  - Output status
  - Manual control
  - Configuration and scheduling

### Automation
- Threshold-based environmental control
- Lighting schedules
- Fan control based on enclosure conditions
- Planned fail-safe logic for overheating or sensor faults

### Future Expansion
- Home Assistant integration
- MQTT or API-based external control
- Historical logging and graphing
- Remote alerting

---

## Project Goals
DragonSense is intended to provide a reliable and extensible control platform for reptile enclosures by combining embedded hardware, sensor monitoring, automation, and a simple user interface.

The initial project scope includes:
- RP2040-based control hardware
- Relay switching for heat and UV sources
- LED and fan control
- Temperature, humidity, and UV sensing
- Local web interface
- A future path toward Home Assistant integration

---

## Hardware Overview

### Core Controller
- RP2040-based board  
  Example: Raspberry Pi Pico or Pico W

### Sensors
- Temperature sensor(s)
- Humidity sensor
- UV sensor

### Outputs
- Relay outputs for switching:
  - UV lights
  - Basking lights
- LED control output
- Fan control output

### Optional Future Hardware
- LCD or OLED status display
- RTC for schedule retention
- External Wi-Fi or use of Pico W
- Buzzer or alarm output for alerts

---

## Software Overview

DragonSense is planned as a modular embedded system with the following major components:

- **Sensor Layer**  
  Reads and validates environmental data

- **Control Layer**  
  Manages relays, fans, and lighting outputs

- **Automation Layer**  
  Applies thresholds, schedules, and safety logic

- **Web Interface**  
  Provides local monitoring and manual control

- **Integration Layer**  
  Planned support for Home Assistant and MQTT

---

## Example Use Cases
- Automatically turn basking lamps on and off on a schedule
- Control enclosure fans when temperature or humidity exceeds limits
- Monitor UV levels for enclosure lighting verification
- View live enclosure conditions from a phone or desktop browser
- Expand into smart-home monitoring and automation platforms

---

## Planned Project Structure

```text
DragonSense/
├── firmware/          # RP2040 firmware source
├── web/               # Web interface assets
├── hardware/          # Schematics, PCB files, wiring diagrams
├── docs/              # Project documentation
├── Repo_Images        # Images used throughout this repo
└── README.md
```

---

## Roadmap
- [ ] RP2040 base firmware
- [ ] Sensor integration
- [ ] Relay output control
- [ ] LED lighting control
- [ ] Fan speed control
- [ ] Web dashboard
- [ ] Configuration storage
- [ ] Data logging
- [ ] Home Assistant integration
- [ ] Local display support

---

## Safety Notes

This project may interface with mains-powered lighting and heating equipment.

Take appropriate precautions:

- Use properly rated relays or switching devices
- Maintain electrical isolation between low-voltage logic and mains circuits
- Include fuse protection where required
- Validate all wiring before connecting live loads
- Design fail-safe behaviour for sensor or control faults
- Always engage a Licenced Electrician for any electrical works
- **No Seriously**, do not attempt any electrical works unless authorised to do so, you could accidentally take the forever nap; or worse, injure you reptile !!

--- 

### Contributing

Contributions, ideas, and improvements are welcome as the project evolves.

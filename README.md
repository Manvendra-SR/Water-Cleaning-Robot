# Water Cleaning Robot

A **3D-printed water-cleaning robot** developed as a team project for the **Design of Machine Elements** course at the Indian Institute of Technology Indore. The prototype combines a front-mounted **rubber conveyor belt** for collecting floating waste with a **two-wheel differential drive** and **Arduino-based Bluetooth control**.

> **Course:** Design of Machine Elements  
> **Project Type:** Team Project  
> **Prototype:** 3D Printed

---

## 🎥 Project Demo

A demonstration video of the working prototype is available here:

**[▶️ Watch the Water Cleaning Robot Demo](https://drive.google.com/file/d/1DYfLFME5Vx7HWMiXFNX8fSm1qkv_5N2b/view?usp=sharing)**

---

## 📌 Overview

The objective of this project was to develop a compact robotic platform capable of moving on a water surface while collecting floating waste.

The robot uses a **front conveyor-belt mechanism** to lift floating waste from the water and move it onto the robot. Locomotion is provided by **two independently driven wheels**, allowing the robot to change its speed and direction. The mechanical structure was fabricated using **3D-printed components**, while an **Arduino, L298N motor driver, DC geared motors, and Bluetooth module** were used for wireless control.

The project demonstrates the integration of:

- Mechanical structure and assembly
- Conveyor-based waste collection
- Differential wheel drive
- DC geared motor actuation
- Arduino-based control
- Bluetooth wireless communication
- Rapid prototyping through 3D printing

---

## 🎯 Objectives

- Develop a mobile platform for collecting floating waste from water bodies.
- Design and integrate a conveyor-based waste collection mechanism.
- Implement independent wheel actuation for speed and directional control.
- Integrate mechanical and electronic subsystems into a functional prototype.
- Demonstrate wireless operation through Bluetooth communication.
- Fabricate and test the prototype using 3D-printed components.

---

## ⚙️ Key Features

| Feature | Implementation |
|---|---|
| Waste Collection | Front-mounted rubber conveyor belt |
| Conveyor Support | Front roller |
| Mobility | Two independently driven wheels |
| Actuation | DC geared motors |
| Controller | Arduino |
| Motor Driver | L298N |
| Wireless Control | Bluetooth module |
| Fabrication | 3D-printed prototype |
| Operation | Wireless mobile control |

---

## 🧩 System Architecture

```text
                    ┌───────────────────────┐
                    │   Mobile Interface    │
                    └───────────┬───────────┘
                                │
                            Bluetooth
                                │
                    ┌───────────▼───────────┐
                    │        Arduino        │
                    │    Control Logic      │
                    └───────┬───────┬───────┘
                            │       │
                            │       │
                 ┌──────────▼───┐   │
                 │ L298N Motor  │   │
                 │    Driver    │   │
                 └──────┬───────┘   │
                        │            │
                  ┌─────┴─────┐     │
                  │           │     │
            ┌─────▼────┐ ┌────▼────┐
            │ Left DC  │ │ Right DC│
            │ Geared   │ │ Geared  │
            │  Motor   │ │  Motor  │
            └──────────┘ └─────────┘

                  Conveyor Drive
                        │
                ┌───────▼────────┐
                │ Rubber Conveyor│
                │ + Front Roller │
                └────────────────┘
```

The exact wiring and control implementation may vary depending on the final prototype configuration.

---

## 🔩 Mechanical Design

The mechanical system consists of the main robot structure, wheel assemblies, and the front waste-collection mechanism.

### Main Mechanical Elements

**1. Robot Structure**  
The main body supports the drive system, conveyor assembly, and electronic components.

**2. Rubber Conveyor Belt**  
A rubber belt is used to transport floating waste from the front of the robot toward the collection side.

**3. Front Roller**  
The front roller supports the conveyor belt and provides the turning path required for continuous belt motion.

**4. Independently Driven Wheels**  
Two side-mounted wheels are independently actuated using DC geared motors. This enables differential control of the robot's motion.

**5. 3D-Printed Components**  
The prototype structure and associated mechanical parts were fabricated using 3D printing, allowing rapid prototyping and straightforward assembly.

---

## 🛞 Drive System

The robot uses **two independently driven DC geared motors**, one on each side.

By varying the relative motion of the two wheels, the robot can achieve different movements:

- **Both wheels forward:** Forward motion
- **Both wheels reverse:** Reverse motion
- **Different wheel speeds:** Turning
- **Opposite wheel directions:** Tight turning/rotation, subject to traction and water-surface conditions

The geared motors provide the torque required to move the prototype while maintaining a controllable operating speed.

---

## 🧹 Conveyor Waste Collection Mechanism

The conveyor is mounted at the front of the robot and is the primary waste-collection mechanism.

### Working Principle

1. The front portion of the conveyor approaches floating waste.
2. The moving rubber belt comes into contact with the waste.
3. The belt carries the material upward and toward the robot.
4. The front roller guides the belt through its continuous motion.
5. The collected material is transferred onto the robot for removal.

This mechanism provides a simple continuous approach to surface-waste collection compared with manually picking individual objects.

---

## 🎮 Control System

The robot is controlled using an **Arduino-based system**.

### Components

- Arduino
- L298N motor driver
- DC geared motors
- Bluetooth communication module
- Conveyor-drive motor/mechanism

The Bluetooth module receives commands from a mobile interface and passes them to the Arduino. The Arduino then controls the motors through the L298N motor driver.

### Control Flow

```text
Mobile App
    │
    │ Bluetooth Commands
    ▼
 Arduino
    │
    ▼
 L298N Motor Driver
    │
    ├───────────────┐
    ▼               ▼
Left Motor      Right Motor

Arduino ─────────► Conveyor Drive
```

This setup allows wireless operation of the robot's drive and conveyor systems.

---

## 🏗️ Fabrication and Assembly

The prototype was fabricated using **3D-printed parts** and assembled as a complete working system.

The overall development involved:

1. Fabrication of the mechanical components
2. Assembly of the robot structure
3. Installation of the wheel and motor assemblies
4. Integration of the conveyor and front roller
5. Mounting of the Arduino and motor driver
6. Connecting the Bluetooth communication system
7. Integrating and testing the complete prototype

The use of 3D printing enabled rapid fabrication and assembly of the prototype.

---

## 🔄 Working Principle

The overall operation can be summarized as follows:

```text
        Wireless Command
               │
               ▼
        Bluetooth Module
               │
               ▼
            Arduino
               │
        ┌──────┴──────┐
        ▼             ▼
   Drive Control   Conveyor Control
        │             │
        ▼             ▼
   Wheel Motors    Conveyor Belt
        │             │
        ▼             ▼
 Robot Movement   Waste Collection
```

During operation, the robot is positioned on the water surface and controlled wirelessly. The drive wheels provide movement and steering while the front conveyor continuously collects floating waste.

---

## 🧰 Components Used

### Mechanical

- 3D-printed structural and mounting components
- Rubber conveyor belt
- Front roller
- Two wheels
- Motor mounts and supports

### Electronics and Actuation

- Arduino board
- L298N motor driver
- DC geared motors
- Bluetooth communication module
- Conveyor-drive motor/mechanism
- Electrical wiring and connectors

> **Note:** Exact motor ratings, battery specification, dimensions, and other numerical specifications are not included because they were not recorded in the available project information.

---

## 👨‍🔧 My Contribution

This was a **team-based project** with responsibilities distributed among team members.

My primary contribution was the **mechanical assembly and structural integration** of the prototype. I worked on joining the fabricated components and integrating the conveyor, front roller, wheel assemblies, and overall robot structure into the complete working prototype.

The individual CAD modeling of the components in **Fusion 360** was primarily handled by another team member, while the prototype assembly and system integration were carried out collaboratively.

---

## 📚 Engineering Concepts Demonstrated

The project provided practical exposure to several mechanical and multidisciplinary concepts:

- Mechanical structure and component integration
- Material handling using conveyor mechanisms
- Differential-drive motion
- Geared motor selection and application
- Mechanical prototyping and 3D printing
- Motor actuation and control
- Basic embedded-system integration
- Wireless control of a robotic platform

---

## ⚠️ Limitations

This project was developed as an academic prototype rather than a production-ready water-cleaning system.

Some limitations include:

- Limited waste-collection capacity due to prototype dimensions
- Performance dependence on the size and type of floating waste
- Mobility affected by water-surface conditions and payload
- No autonomous navigation or obstacle avoidance
- No onboard waste-capacity sensing
- No documented measurements for collection rate, operating speed, battery life, or payload capacity

---

## 🚀 Possible Improvements

### Mechanical Improvements

- Increase conveyor width and collection area
- Add a dedicated waste-storage container
- Improve structural rigidity and waterproofing
- Optimize conveyor geometry for different waste sizes
- Improve buoyancy distribution and stability

### Mobility Improvements

- Improve wheel traction and propulsion efficiency
- Use higher-torque or more efficient motors where necessary
- Add stabilization or guidance mechanisms
- Optimize the hull/body geometry for lower water resistance

### Control Improvements

- Add autonomous navigation
- Introduce obstacle-detection sensors
- Implement feedback-based motor control
- Add battery and system-status telemetry
- Integrate water-quality or environmental sensors

---

## 🙏 Acknowledgements

This project was completed as a team project for the **Design of Machine Elements** course at the **Indian Institute of Technology Indore**.

The project involved collaborative work across mechanical assembly, fabrication, actuation, electronics, and control.

---

## 📄 Disclaimer

This README documents the academic prototype based on the available project information. Detailed numerical specifications, circuit diagrams, CAD files, testing data, and performance measurements should be added when the corresponding project records are available.

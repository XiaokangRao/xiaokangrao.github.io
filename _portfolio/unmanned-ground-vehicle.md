---
title: "UGV Autonomous Navigation & Intelligent Inspection System"
excerpt: "Development of an integrated positioning, localisation and navigation system for unmanned ground vehicles."
collection: portfolio
---

## Overview

**Autonomous Ground Vehicle | GNSS-RTK Integration | Multi-Sensor Fusion | ROS 2 | Robotics | Mobile Surveying**

An integrated Unmanned Ground Vehicle (UGV) platform combining high-precision GNSS-RTK positioning, multi-sensor perception, state estimation, SLAM, and autonomous navigation.

The platform integrates GNSS-RTK, IMU, wheel odometry, LiDAR, and depth cameras to achieve robust localisation, continuous positioning, environmental perception, and autonomous mobility in indoor and outdoor environments.

By integrating geodetic positioning technologies with robotics and multi-sensor fusion, this project explores autonomous inspection, mobile surveying, and intelligent geospatial data acquisition.

## System Architecture

![UGV System Architecture](/images/ugv/ugv_architecture.png)

The system consists of four major layers:

1. **UGV Hardware & Multi-Sensor Integration** – mobile robot platform, GNSS-RTK, IMU, wheel encoders, LiDAR, depth cameras, and embedded computing.
2. **Positioning & Multi-Sensor Fusion** – GNSS-RTK integration, EKF-based state estimation, factor graph optimisation, and robot localisation.
3. **SLAM & Autonomous Navigation** – ROS 2, environmental perception, mapping, localisation, path planning, and motion control.
4. **Engineering Applications** – autonomous inspection, mobile surveying, and geospatial data acquisition.

## UGV Hardware Development

Development and integration of a multi-sensor unmanned ground vehicle platform.

### Mobile Robot Platform

- UGV chassis and mobile robotic platform
- Wheel-based drive system and motion control
- Embedded computing and hardware integration
- Sensor installation and calibration
- Power supply and system integration
- ROS 2-compatible hardware interfaces

### Multi-Sensor Configuration

| Hardware | Function |
|---|---|
| GNSS-RTK Receiver | High-precision global positioning |
| GNSS Antenna | Satellite signal acquisition |
| IMU | Acceleration and angular velocity measurements |
| Wheel Encoders | Wheel odometry and motion estimation |
| LiDAR | Environmental perception and spatial mapping |
| Depth Camera | RGB-D sensing and 3D scene perception |
| Embedded Computer | Robot processing and system coordination |

### GNSS-RTK Integration with UGV

A key feature of the platform is the integration of GNSS-RTK positioning with the mobile robotic system.

- GNSS-RTK receiver and antenna integration
- RTK correction data acquisition
- Global positioning and coordinate estimation
- GNSS data integration with ROS 2
- Coordinate transformation between GNSS and robot frames
- Time synchronisation and sensor data integration
- Outdoor positioning and navigation

This integration connects geodetic positioning with robotic localisation, enabling globally referenced mobile navigation and spatial data acquisition.

## Multi-Sensor Fusion & Localisation

Integration of complementary sensors to improve positioning accuracy, continuity, and robustness.

### Sensor Fusion Architecture

- GNSS-RTK global positioning
- IMU-based motion estimation
- Wheel odometry integration
- LiDAR-based localisation
- Depth camera-based environmental perception
- Multi-sensor calibration and synchronisation
- Coordinate frame transformation

### State Estimation & Optimisation

- Extended Kalman Filter (EKF)
- GNSS–IMU–Wheel Odometry integration
- LiDAR-assisted localisation
- Robot pose and state estimation
- Factor graph optimisation
- Trajectory estimation and optimisation
- Global and local localisation

### Positioning Framework

```text
       GNSS-RTK
           │
           ▼
    Global Positioning
           │
           │
IMU ───────┤
           │
Wheel ─────┤
Odometry   │
           │
LiDAR ─────┤
           ▼
    Multi-Sensor Fusion
           │
     ┌─────┴─────┐
     ▼           ▼
    EKF     Factor Graph
     │           │
     └─────┬─────┘
           ▼
    Robot Pose Estimation
       (x, y, θ)
           │
           ▼
   Global & Local Localisation
```

GNSS-RTK provides global positioning references, while IMU, wheel odometry, and LiDAR provide complementary motion and local positioning information. Their integration supports continuous state estimation and robust navigation in different operating environments.

## SLAM & Environmental Perception

Implementation and evaluation of SLAM and localisation frameworks for robotic environmental perception.

### SLAM Frameworks

- **GMapping** – 2D occupancy grid mapping using LiDAR and odometry.
- **Google Cartographer** – LiDAR-based SLAM, scan matching, and pose estimation.
- **SLAM Toolbox** – mapping, localisation, and map management.

### Core Capabilities

- LiDAR-based environmental perception
- Real-time robot localisation
- 2D occupancy grid mapping
- Point cloud processing
- Scan matching
- Loop closure
- Map-based localisation
- Integration with navigation modules

The SLAM frameworks support local mapping and localisation, complementing GNSS-RTK global positioning for indoor and outdoor robotic applications.

## Autonomous Navigation & Motion Control

Integration of localisation, environmental perception, and navigation components for autonomous UGV operation.

### Navigation Capabilities

- Global and local localisation
- GNSS-assisted outdoor navigation
- Map-based navigation
- Global and local path planning
- Obstacle detection and avoidance
- Path following
- Closed-loop motion control
- Autonomous waypoint navigation

### Navigation Workflow

```text
Multi-Sensor Data Acquisition
            │
            ▼
      Robot Localisation
            │
            ▼
    Environment Perception
            │
            ▼
       Path Planning
            │
            ▼
    Obstacle Avoidance
            │
            ▼
     Motion Control
            │
            ▼
    Autonomous Navigation
```

## Autonomous Inspection & Mobile Surveying

Application of the integrated UGV platform to infrastructure inspection, mobile measurement, and geospatial data acquisition.

### Autonomous Inspection

- Autonomous route following
- Sensor-based environmental inspection
- LiDAR-based obstacle detection
- Inspection waypoint navigation
- Remote robot monitoring
- Indoor and outdoor inspection scenarios

### Mobile Surveying & Geospatial Data Acquisition

- GNSS-RTK-based global positioning
- LiDAR-based spatial mapping
- Depth camera-based 3D perception
- Robot trajectory estimation
- Georeferenced mapping
- Mobile spatial data acquisition
- Integration of positioning and mapping information

### Application Scenarios

| Application | Technical Capabilities |
|---|---|
| Infrastructure Inspection | Autonomous navigation and environmental sensing |
| Mobile Mapping | LiDAR and depth camera integration |
| Geospatial Surveying | GNSS-RTK positioning and trajectory estimation |
| Outdoor Robotics | GNSS-assisted autonomous navigation |
| Spatial Data Acquisition | Positioning and 3D environmental perception |

## Technology Stack

### Hardware & Embedded Systems

- UGV mobile platform
- GNSS-RTK receiver and antenna
- IMU sensors
- Wheel encoders
- LiDAR
- Depth cameras
- Embedded computing

### Robotics & Middleware

- ROS 2
- Linux / Ubuntu
- TF2 coordinate transformations
- ROS 2 sensor integration
- Robot state estimation
- Robotics communication and control

### Positioning & Sensor Fusion

- GNSS-RTK
- Extended Kalman Filter (EKF)
- Factor Graph Optimisation
- GNSS–IMU Integration
- Wheel Odometry
- LiDAR-based Localisation
- Sensor Calibration and Synchronisation

### SLAM & Navigation

- GMapping
- Google Cartographer
- SLAM Toolbox
- Occupancy Grid Mapping
- Scan Matching
- Robot Localisation
- Path Planning
- Obstacle Avoidance

### Data Processing & Visualisation

- Python
- C++
- ROS 2 Visualisation
- RViz2
- Point Cloud Processing
- Trajectory Analysis
- Spatial Data Visualisation

## System Development Workflow

```text
UGV Hardware Development
            │
            ▼
Multi-Sensor Integration
            │
            ▼
GNSS-RTK / IMU / Wheel / LiDAR
            │
            ▼
Sensor Calibration & Synchronisation
            │
            ▼
Multi-Sensor Fusion & Localisation
            │
            ▼
SLAM & Environmental Perception
            │
            ▼
Autonomous Navigation
            │
            ▼
Mobile Inspection & Surveying
            │
            ▼
Geospatial Data Acquisition
```

## Project Highlights

- **GNSS-RTK and Robotics Integration:** Integration of high-precision GNSS positioning with a mobile robotic platform.
- **Multi-Sensor Hardware Development:** Integration of GNSS-RTK, IMU, wheel encoders, LiDAR, and depth cameras.
- **Robust Localisation:** Multi-sensor state estimation using EKF and factor graph-based optimisation approaches.
- **ROS 2 Robotics Development:** Integration of sensor drivers, coordinate transformations, localisation, and navigation modules.
- **SLAM and Environmental Perception:** Implementation and evaluation of GMapping, Cartographer, and SLAM Toolbox.
- **Autonomous Navigation:** Integration of positioning, perception, path planning, and motion control.
- **Engineering Applications:** Autonomous inspection, mobile surveying, and geospatial data acquisition.

## Project Status

This repository documents the development and integration of a GNSS-RTK-enabled UGV platform, including hardware integration, ROS 2 software, multi-sensor fusion, localisation, SLAM, navigation, and field experiments.

Individual components and system-level performance are under continuous development and validation.

## Research Interests

`UGV` · `GNSS-RTK` · `Mobile Robotics` · `ROS 2` · `Multi-Sensor Fusion` · `EKF` · `Factor Graph` · `SLAM` · `Robot Localisation` · `Autonomous Navigation` · `LiDAR` · `Depth Camera` · `IMU` · `Wheel Odometry` · `Mobile Mapping` · `Geospatial Engineering`
## Project Outcomes

Development of a multi-sensor UGV positioning and navigation platform, enabling investigation of high-precision localisation, sensor fusion and autonomous navigation in real-world environments.

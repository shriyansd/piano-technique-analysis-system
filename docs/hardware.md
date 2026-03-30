# Hardware System

## Overview
The system uses a lightweight sensor-equipped glove connected to an external module to capture finger interaction, hand posture, and motion during piano playing while preserving natural movement.

## Components

### Finger Sensors (FSR)
- 5 force-sensitive resistors placed on fingertips  
- Measure press timing and relative force at the point of key contact, enabling analysis of attack and consistency

### Motion Sensor (IMU)
- Mounted on top of glove (back of hand or wrist)  
- Tracks wrist angle, hand rotation, and motion without interfering with key interaction

### Posture Sensor (Flex Sensor)
- Placed across the hand arch (exact placement TBD: palm vs knuckle region)  
- Measures curvature of the hand to capture posture and detect collapse of technique

### Audio Input (Microphone)
- Detects note onset timing  
- Enables comparison between physical key press and actual sound produced

### External Module
- Contains microcontroller (Arduino Nano or similar)  
- Connected via wired cable anchored near the wrist to remove weight from the glove and maintain comfort

## Design Principles
- Maintain a lightweight, unobtrusive glove  
- Avoid interference with natural playing technique  
- Focus on collecting reliable, meaningful data rather than maximizing complexity

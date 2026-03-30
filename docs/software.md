# Software System

## Overview
The software processes sensor data from the glove to analyze piano technique and provide real-time and post-session feedback.

## Data Flow
Glove Sensors → Microcontroller → Laptop → Processing → Visualization

## Capabilities

### Timing Analysis
- Combines FSR (finger press), microphone (sound onset), and MIDI input (expected timing and note identity)  
- Measures early/late notes, delay between press and sound, and overall synchronization accuracy

### Finger Consistency Analysis
- Tracks variation in force and timing across repetitions  
- Identifies weaker or inconsistent fingers and uneven playing patterns

### Posture Analysis
- Uses IMU for wrist angle and motion and flex sensor for hand curvature  
- Detects hand collapse, wrist drop, and unnecessary movement during playing

## Considerations

### Synchronization
- Aligns timing across FSR, microphone, and MIDI data to ensure accurate comparisons

### Calibration
- Establishes baseline values and thresholds for sensors  
- Normalizes readings across fingers for consistent measurement

### Signal Processing
- Filters noise from sensor inputs and applies thresholds for stable detection

## Future Features
- MIDI-based performance comparison  
- Structured exercise analysis  
- Session summaries and progress tracking

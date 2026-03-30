# Week 1 — Project Planning and System Design

## Sunday - Day 1
- Conceptualized a wearable glove to analyze piano technique
  - 5 FSR sensors on fingertips to measure force at key contact (directly captures timing and attack behavior)
  - 1 flex sensor (placement TBD: palm vs knuckle region) to detect hand posture/arch (important for identifying technique issues like      collapse)
  - IMU on top of glove to track wrist angle and motion without interfering with key interaction
  - External module (Arduino Nano) connected at wrist to keep glove lightweight and preserve natural hand movement
  - MIDI input used for accurate note identity and expected timing reference
  - Microphone used for note onset detection to compare physical press vs actual sound

- Identified key focus areas:
  - Timing accuracy  
    - Combine FSR (press), microphone (sound onset), and MIDI (expected timing)  
    - Measure delay, early/late playing, and synchronization  
  - Finger consistency  
    - Use FSR data to track variation in force and timing across repetitions  
    - Identify weaker or lagging fingers (ex: ring/pinky)  
    - Essential for even and controlled playing  
  - Posture  
    - Use flex sensor for hand arch and IMU for wrist angle and motion  
    - Detect issues such as hand collapse, wrist drop, and unnecessary movement  
    - Poor posture reduces control and leads to inconsistent or inefficient technique
  - Calibration  
    - Determine baseline and threshold values for FSR sensors  
    - Normalize force readings across different fingers  
    - Calibrate IMU orientation for consistent posture tracking
  - Scope constraints  
    - Initial system will focus on structured exercises or limited note ranges  
    - Full note identification from audio will not be attempted initially  
    - Why: prioritizes reliability and feasibility over complexity in early versions  

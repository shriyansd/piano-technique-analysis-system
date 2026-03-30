# Project Overview

## Concept
This project is a wearable system designed to analyze piano technique using real-time sensor data. A glove equipped with sensors captures how a pianist interacts with the instrument, focusing on timing, control, and posture.

## Motivation
Piano technique is often taught and evaluated subjectively. This system aims to provide measurable insights into performance, allowing players to understand and improve their technique more effectively.

## What the System Measures

### Timing
Evaluates when notes are played relative to expected timing, using sensor data and audio signals.

### Finger Control
Analyzes how consistently each finger applies force and timing across repeated notes.

### Posture
Tracks hand shape and wrist position to identify inefficient or incorrect technique.

## System Approach
The glove collects data from multiple sensors, which is transmitted to a computer for processing. The system compares physical interaction (finger press), sound output, and expected input (MIDI) to generate performance insights.

## Key Design Goals
- Keep the glove lightweight and non-intrusive  
- Capture meaningful aspects of technique, not just note correctness  
- Prioritize reliability and clarity over complexity in early stages  

## Current Scope
The initial version focuses on:
- timing accuracy  
- finger consistency  
- posture detection  

More advanced features will be added as the system develops.

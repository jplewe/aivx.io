---
layout: page
title: AIVX ENGINE
permalink: /engine/
nav: false
---

Here's a Cursor-generated summary of my progress on the engine so far. (It's codenamed Wave internally.) All of this has been added on top of Godot.

## AIVX Engine - Interactive Experience Framework

A sophisticated game engine and application framework built in **Godot 4** using **C#**, designed for creating modular, extensible interactive experiences with a focus on visual and audio aesthetics.

## Project Overview

AIVX Engine is a comprehensive framework that provides a unified platform for developing various types of games and applications. It features a modular architecture with shared infrastructure for common functionality, allowing developers to rapidly prototype and build interactive experiences.

## Core Architecture

### WaveOS - The Operating System Layer
The central orchestrator that manages the entire application ecosystem:

- **Application Lifecycle** - Launching, switching, and destroying applications
- **Input Management** - Unified input handling across keyboard, mouse, gamepad, and VR
- **Rendering System** - Camera management, environment settings, shader parameters
- **Audio/Video Systems** - Background audio and video playback
- **Fade Effects** - Smooth transitions between applications

### WaveObject - Base Class System
All game objects inherit from `WaveObject`, providing:

- **Transform Management** - Position, rotation, scale with helper methods
- **Lifecycle Hooks** - `WaveInit()`, `WaveUpdate()`, `WaveDestroy()`
- **Material/Shader Management** - Unified material and shader assignment
- **Color System** - Integrated color management with ID-based color lookup
- **Bounds and Collision** - Automatic bounding box calculations

### WaveApp - Application Framework
Applications inherit from `WaveApp` and provide:

- **Menu Systems** - Built-in UI management
- **State Management** - Game states, pause/resume functionality
- **Input Handling** - App-specific input processing

## Key Systems

### AI System (WaveAI)
- **ChatGPT Integration** - Direct API integration with OpenAI's GPT models
- **Function Calling** - Structured function schemas for data visualization
- **Database Management** - AI-powered database selection and loading
- **Presentation Generation** - Automated slide creation with narration
- **Data Analysis** - AI-driven insights and statistical analysis
- **Natural Language Interface** - Conversational interaction with the system

### Input System (WaveIn)
- **Unified Input Mapping** - Supports keyboard, mouse, gamepad, and VR controllers
- **Action-Based Input** - Abstracted input actions like "accept", "back", "action1"
- **Multi-Device Support** - Seamless switching between input methods
- **Raycasting** - 3D mouse interaction with colliders

### Generation System (WaveGen)
- **Object Factories** - `GenObject<T>()`, `GenCube()`, `GenText()`
- **Mesh Generation** - Procedural mesh creation (cubes, spheres, grids)
- **Material Creation** - Automatic material assignment with shaders
- **Pooling System** - Object pooling for performance

### Visual System
- **Shader Management** - Extensive shader system with custom effects
- **Color Schemes** - Triadic color generation, random color sets
- **Camera System** - Follow targets, lerp movement, zoom controls
- **Environment Effects** - Fog, glow, sky colors

### Audio/Video System
- **Background Audio** - Ambient music and sound management
- **Video Playback** - Background video support
- **Audio Visualization** - Real-time audio analysis



## Technical Features

### Shader System
- **Custom Shaders** - hexdots, meta, skycolor, energyball effects
- **Dynamic Shader Parameters** - Real-time shader modification
- **Visual Effects** - Glow, pulse, scrolling lines, edge effects

### Performance Optimizations
- **Object Pooling** - `WavePool<T>` for efficient object reuse
- **Lazy Initialization** - Components initialize only when needed
- **Render Priorities** - Controlled rendering order

### VR Support
- **OpenXR Integration** - VR headset and controller support
- **XR Input Mapping** - VR-specific input handling
- **Stereoscopic Rendering** - VR-compatible rendering pipeline



## How It Works

1. **Startup** - `metagame.cs` initializes the system, creating a `WaveOS` instance
2. **Launcher** - `LauncherApp` provides the main menu for selecting applications
3. **App Switching** - `WaveOS.LaunchApp<T>()` destroys current app and launches new one
4. **Input Processing** - `WaveIn` processes all input and maps to abstract actions
5. **AI Integration** - `WaveAI` provides ChatGPT integration and function calling
6. **Rendering** - Custom shaders provide visual effects, with global shader parameters
7. **Audio/Video** - Background systems provide ambient audio and video

## Development Philosophy

The framework is designed for **rapid prototyping** and development of interactive experiences, with a focus on:

- **Modularity** - Each application can be developed independently
- **Reusability** - Shared infrastructure for common functionality
- **Performance** - Optimized rendering and object management
- **Extensibility** - Easy to add new applications and features
- **Visual Appeal** - Rich shader system and visual effects
- **AI Integration** - Seamless AI-powered features and natural language interaction
- **Data Intelligence** - Automated data analysis and visualization generation

## Use Cases

- **Game Development** - Rapid prototyping of various game types
- **Interactive Art** - Visual and audio experiences
- **Educational Tools** - Interactive learning applications
- **VR Experiences** - Immersive virtual reality applications
- **Audio Visualization** - Real-time audio analysis and visualization
- **Data Visualization** - AI-powered data analysis and presentation generation
- **Business Intelligence** - Automated report creation and data insights
- **Research Tools** - Statistical analysis and data exploration

---

*AIVX Engine represents a comprehensive approach to interactive experience development, providing the tools and infrastructure needed to create engaging, visually stunning applications with minimal boilerplate code.*
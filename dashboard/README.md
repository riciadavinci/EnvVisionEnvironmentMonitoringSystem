<!-- Main Header -->
<a id="heading"></a>

# _EnvDash_ - Dashboard for _EnvVision_ Environment Monitoring System

<!-- Badges & Shields -->
[![C++20](https://img.shields.io/badge/C%2B%2B-20-blue.svg)](https://en.cppreference.com/w/cpp/20)
[![Qt 6.8+](https://img.shields.io/badge/Qt-6.8%2B-007ACC.svg?logo=qt)](https://www.qt.io/)
[![CMake](https://img.shields.io/badge/CMake-3.25%2B-064F8C.svg?logo=cmake)](https://cmake.org/)
[![Build Status](https://github.com/riciadavinci/EnvVisionEnvironmentMonitoringSystem/actions/workflows/ci-dashboard.yml/badge.svg)](https://github.com/riciadavinci/EnvVisionEnvironmentMonitoringSystem/actions)
[![codecov](https://codecov.io/gh/riciadavinci/EnvVisionEnvironmentMonitoringSystem/graph/badge.svg?token=YOUR_TOKEN)](https://codecov.io/gh/riciadavinci/EnvVisionEnvironmentMonitoringSystem)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)


<!-- Elevator Pitch -->
<a id="elevator-pitch"></a>

## 1. Elevator Pitch

<p align="right"><sub>[&nbsp;<a href="#heading">Back to Top</a> &nbsp;•&nbsp; <a href="#table-of-contents">Table of Contents</a>&nbsp;]</sub></p>


<!-- Visual Preview / Gallery (Screenshots/GIFs placeholder) -->
<a id="gallery"></a>

## 2. Gallery

<!-- Dashboard Rough Sketch -->
<figure>
    <img src="docs/assets/EnvironmentMonitorDashboardRoughSketch.png" 
         alt="Dashboard Rough Sketch" height="350">
    <figcaption>Dashboard Rough Sketch</figcaption>
</figure>

<p align="right"><sub>[&nbsp;<a href="#heading">Back to Top</a> &nbsp;•&nbsp; <a href="#table-of-contents">Table of Contents</a>&nbsp;]</sub></p>


<!-- Table of Contents -->
<a id="table-of-contents"></a>

## Table of Contents
| # | Section |
|---|---|
| **1.** | [Elevator Pitch](#elevator-pitch) |
| **2.** | [Gallery](#gallery) |
| **3.** | [Key Technical Features](#key-technical-features) |
| **4.** | [System Architecture & Design Patterns](#system-architecture-and-design-patterns) |
|  | 4.1 &emsp;[Sub-Section 1](#) |
|  | 4.2 &emsp;[Sub-Section 2](#) |
|  | 4.3 &emsp;[Sub-Section 3](#) |
| **5.** | [Tech Stack & Module Matrix](#tech-stack-and-module-matrix) |
| **6.** | [Build & Development Setup](#build-and-development-setup) |
| **7.** | [Project Scope & Roadmap](#project-scope-and-roadmap) |
|  | 7.1 &emsp;[Project Scope](#project-scope) |
|  | 7.2 &emsp;[Project Roadmap](#project-roadmap) |
| **8.** | [Testing & Static Analysis](#testing-and-static-analysis) |

<p align="right"><sub>[&nbsp;<a href="#heading">Back to Top</a> &nbsp;•&nbsp; <a href="#table-of-contents">Table of Contents</a>&nbsp;]</sub></p>


<!-- Key Technical Features (What makes this hard/interesting?) -->
<a id="key-technical-features"></a>

## 3. Key Technical Features

<p align="right"><sub>[&nbsp;<a href="#heading">Back to Top</a> &nbsp;•&nbsp; <a href="#table-of-contents">Table of Contents</a>&nbsp;]</sub></p>


<!-- System Architecture & Design Patterns (The technical proof) -->
<a id="system-architecture-and-design-patterns"></a>

## 4. System Architecture & Design Patterns

<p align="right"><sub>[&nbsp;<a href="#heading">Back to Top</a> &nbsp;•&nbsp; <a href="#table-of-contents">Table of Contents</a>&nbsp;]</sub></p>


<!-- Tech Stack & Module Matrix -->
<a id="tech-stack-and-module-matrix"></a>

## 5. Tech Stack & Module Matrix

<p align="right"><sub>[&nbsp;<a href="#heading">Back to Top</a> &nbsp;•&nbsp; <a href="#table-of-contents">Table of Contents</a>&nbsp;]</sub></p>


<!-- Build & Development Setup (Windows MSVC/MinGW & Linux setup) -->
<a id="build-and-development-setup"></a>

## 6. Build & Development Setup

<p align="right"><sub>[&nbsp;<a href="#heading">Back to Top</a> &nbsp;•&nbsp; <a href="#table-of-contents">Table of Contents</a>&nbsp;]</sub></p>


<!-- V1.0.0 Scope, Roadmap & Progress (Checklist showing project management skill) -->
<a id="project-scope-and-roadmap"></a>

## 7. Project Scope & Roadmap


<a id="project-scope"></a>

### 7.1 Project Scope (Component: Dashboard - _EnvDash_)

The primary objective of **_EnvDash_** is to provide a real-time desktop interface for visualizing environmental sensor telemetry originating from hardware nodes (Pico 2 firmware) or simulated environments/mock hardware (Python).

#### In-Scope (v1.0 Deliverables)
* **Real-Time Telemetry Visualization:** Live rendering of temperature, humidity, and atmospheric metrics using Qt Quick / QML widgets and dynamic charts.
* **Multi-Transport Support:** Data ingestion over Serial (UART/USB) for physical hardware connections and IPC/Local Sockets for communication with the Python mock hardware simulator.
* **Hardware Status Monitoring:** UI indicators for connection state, packet loss, transmission frequency, and system threshold alerts.
* **Configurable Dashboard Settings:** Controls enabling users to adjust sample rates, threshold triggers, and chart timeframes dynamically.
* **Cross-Platform Target:** Build targets verified on both Windows (MSVC/MinGW) and Linux (GCC) environments.

<br>

#### Out-of-Scope (v1.0 Non-Goals)
* **Cloud Storage & Remote Sync:** No direct backend cloud integration (AWS/Azure) or remote database persistence for v1.0; logging is handled locally.
* **Mobile / Web Platforms:** Exclusive focus on desktop environments (no iOS, Android, or WebAssembly targets).
* **User Authentication:** Single-user local desktop application without user login or permission roles.
* **Direct Firmware Flashing:** The application consumes telemetry streams only and does not perform OTA or direct firmware flashing to the microcontroller.


<p align="right"><sub>[&nbsp;<a href="#heading">Back to Top</a> &nbsp;•&nbsp; <a href="#table-of-contents">Table of Contents</a>&nbsp;]</sub></p>


<a id="project-roadmap"></a>

### 7.2 Project Roadmap (Component: Dashboard _EnvDash_)
- [ ] **Feature:** Setup Project Skeleton. Define project scope, features & tasks
    - [x] ✔️ **Task:** Setup minimal CI/CD script with test job &emsp;<small>[&nbsp; **Completed:** 31.07.2026 &nbsp;|&nbsp; **Author:** [@riciadavinci](https://github.com/riciadavinci) &nbsp;]</small>
    - [x] ✔️ **Task:** Define project scope &emsp;<small>[&nbsp; **Completed:** 01.08.2026 &nbsp;|&nbsp; **Author:** [@riciadavinci](https://github.com/riciadavinci) &nbsp;]</small>
    - [x] ✔️ **Task:** Define project features and tasks loosely &emsp;<small>[&nbsp; **Completed:** 01.08.2026 &nbsp;|&nbsp; **Author:** [@riciadavinci](https://github.com/riciadavinci) &nbsp;]</small>
    - [ ] **Task:** Create main.qml and use it with main.cpp
    - [ ] **Task:** Setup CMakeLists.txt to compile for main.cpp
    - [ ] **Task:** Create simple GUI App that builds successfully
- [ ] **Feature:** Setup Full CI/CD Pipeline
    - [ ] **Task:** Setup working CMake Build Task
    - [ ] **Task:** Setup working Clang-Tidy Analysis
    - [ ] **Task:** Setup Google Test
    - [ ] **Task:** Setup Unit-Tests execution
    - [ ] **Task:** Setup GCov/LCov Coverage Report Generation
- [ ] **Feature:**
    - [ ] **Task:** 

<!-- - [ ] **Feature:** Setup Full CI/CD Pipeline &emsp;[&nbsp; **Completed:** 11.06.2026 &nbsp;|&nbsp; **Merge/PR:** [a3f1f66](https://github.com/riciadavinci/EnvVisionEnvironmentMonitoringSystem/commit/a3f1f66b9da4bb4b6993f7b7090cecea019e56a8) &nbsp;]
    - [x] **Task:** Setup minimal skeleton with Sample Job &emsp;[&nbsp; **Completed:** 01.08.2026 &nbsp;|&nbsp; **Author:** [@riciadavinci](https://github.com/riciadavinci) &nbsp;]
	- [ ] **Task:** Setup Clang-Tidy Static Analysis Job
- [ ] **Feature:** Setup CMakeLists.txt and Source Files Skeleton -->

<p align="right"><sub>[&nbsp;<a href="#heading">Back to Top</a> &nbsp;•&nbsp; <a href="#table-of-contents">Table of Contents</a>&nbsp;]</sub></p>


<!-- Testing & Static Analysis -->
<a id="testing-and-static-analysis"></a>

## 8. Testing & Static Analysis



<p align="right"><sub>[&nbsp;<a href="#heading">Back to Top</a> &nbsp;•&nbsp; <a href="#table-of-contents">Table of Contents</a>&nbsp;]</sub></p>

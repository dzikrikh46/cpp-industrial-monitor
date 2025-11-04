# cpp-industrial-monitor
# C++ Industrial Monitoring System

A modern industrial monitoring system built with a C++ backend and a web-based frontend. This project demonstrates a real-time data pipeline from a C++ simulation to a dynamic web dashboard.

## Features

- [ ] Real-time sensor data simulation (Temperature, Pressure, etc.).
- [ ] RESTful API built with C++ and the Crow library.
- [ ] Interactive web dashboard with real-time charts using Chart.js.
- [ ] Thread-safe data handling between the simulator and the web server.

## Tech Stack

**Backend:**
- C++17
- [Crow](https://github.com/CrowCpp/Crow) (C++ microframework)
- [nlohmann/json](https://github.com/nlohmann/json) (JSON library for Modern C++)
- CMake (Build System)
- vcpkg (Package Manager)

**Frontend:**
- HTML5
- CSS3
- JavaScript (ES6+)
- [Chart.js](https://www.chartjs.org/) (Data visualization)

## How to Run

This project is designed to run in [GitHub Codespaces](https://github.com/features/codespaces).

1. Click the green `<> Code` button on this repository.
2. Select the `Codespaces` tab and click `New codespace`.
3. Wait for the environment to be built (this may take a few minutes on the first run).
4. Once ready, open a terminal in VS Code and run:
   ```bash
   cmake -B build -S . && cmake --build build
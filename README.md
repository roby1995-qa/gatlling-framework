# gatlling-framework
# Gatling Performance Testing Framework

## Overview
This framework is designed for performance testing using Gatling. It includes a basic simulation setup, supports HTTP protocols, and is easily extendable for advanced performance testing scenarios.

---

## Features
- **Easy-to-Use Structure:** Organized for quick integration and execution.
- **Scalable Simulations:** Supports various load injection models.
- **Real-Time Metrics:** Provides detailed insights into performance bottlenecks.
- **HTML Reports:** Automatically generates reports after each test execution.
- **Modular Configuration:** Simplifies updates and customizations.

---

## Prerequisites

1. **Install Java:**
   Ensure JDK 8 or later is installed on your system.
   ```bash
   java -version
2. Install SBT: SBT (Scala Build Tool) is required for managing dependencies and executing simulations.


sbt sbtVersion
Install Gatling Plugin: Gatling plugin is integrated through SBT in the framework.

Set Up Dependencies: Dependencies are managed in build.sbt.

3. GatlingPerformanceFramework/
├── src/
│   ├── test/
│   │   ├── resources/
│   │   │   ├── logback.xml         # Logging configuration
│   │   ├── scala/
│   │   │   ├── simulations/
│   │   │   │   ├── BasicSimulation.scala # Sample simulation
├── build.sbt                       # SBT build configuration
├── README.md                       # Documentation


Running Tests
Compile the Project: Compile the project using SBT to ensure all dependencies are installed.


sbt compile
Execute Simulations: Run all simulations in the simulations/ folder.

sbt gatling:test
View Reports: HTML reports are generated in the target/gatling directory. Open the index.html file for detailed metrics.

Framework Structure
Simulations Folder
This folder contains all simulation scripts. Each script represents a performance test scenario.

Resources Folder
The resources/ directory includes configuration files like logback.xml.

build.sbt
This file defines the project setup, dependencies, and plugins.

Debugging
Logs: Check the console output or logs in the target/gatling directory.
Errors: Resolve compilation or runtime errors by reviewing the simulation scripts and SBT dependencies.

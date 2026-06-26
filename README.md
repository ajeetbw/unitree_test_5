# Unitree Robot SDK Version 2
Unitree Robot SDK Version 2 is a comprehensive software development kit designed to provide a seamless and efficient way to interact with Unitree robots. This SDK is built on top of a robust architecture, allowing developers to create innovative applications and integrate Unitree robots into various projects.

## Project Description
The Unitree Robot SDK Version 2 is designed to provide a unified interface for controlling and interacting with Unitree robots. It offers a wide range of features, including motion control, sensor integration, and communication protocols. This SDK is ideal for developers, researchers, and engineers who want to create custom applications, simulate robot behavior, or integrate Unitree robots into existing systems.

## Tech Stack
The Unitree Robot SDK Version 2 is built using a combination of cutting-edge technologies, including:
* **Programming Languages:** C++, Python
* **Frameworks:** CMake, Eigen, Boost
* **Libraries:** YAML-CPP, SPDLOG, FMT
* **Operating Systems:** Ubuntu 20.04 LTS (supported on both aarch64 and x86_64 architectures)

## Installation and Startup
To get started with the Unitree Robot SDK Version 2, follow these steps:
### Prerequisites
* Install the required dependencies: `apt-get update` and `apt-get install -y cmake g++ build-essential libyaml-cpp-dev libeigen3-dev libboost-all-dev libspdlog-dev libfmt-dev`
* Ensure you have the necessary compiler (GCC version 9.4.0) and CMake (version 3.10 or higher) installed

### Building the SDK
```bash
mkdir build
cd build
cmake ..
make
```

### Installing the SDK
To install the SDK system-wide:
```bash
sudo make install
```
Alternatively, you can install the SDK to a custom directory:
```bash
cmake .. -DCMAKE_INSTALL_PREFIX=/opt/unitree_robotics
sudo make install
```
Note that if you install the library to a non-standard location, you need to add the path to `${CMAKE_PREFIX_PATH}` so that CMake can find it using `find_package()`.

## Basic Usage
The Unitree Robot SDK Version 2 provides a range of examples to demonstrate its capabilities. For instance, you can use the `example/cmake_sample` to learn how to import the SDK into your CMake project.

### State Machine Example
The `example/state_machine` directory contains an example that showcases the SDK's state machine capabilities. You can modify the `params.json` file to adjust the parameters:
```json
{
    "dt": 0.01,
    "kp": 40.0,
    "kd": 1.0,
    "init_pos": [
        0.0,
        0.9,
        -1.8,
        0.0,
        0.9,
        -1.8,
        0.0,
        0.9,
        -1.8,
        0.0,
        0.9,
        -1.8
    ]
}
```
### H1_2 Parallel Mechanism Control Example
The `example/h1` directory contains an example that demonstrates the H1_2 parallel mechanism control interface. You can use this example to learn how to control the robot's ankle joints.

## Contributing
We welcome contributions to the Unitree Robot SDK Version 2. If you're interested in contributing, please fork this repository and submit a pull request with your changes.

## Licensing
The Unitree Robot SDK Version 2 is licensed under [insert license]. By contributing to this project, you agree to release your contributions under the same license.

## Additional Resources
For more information about the Unitree Robot SDK Version 2, please visit the [Unitree Document Center](https://support.unitree.com/home/zh/developer).
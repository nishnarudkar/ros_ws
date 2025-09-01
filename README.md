# ros_ws

This repository contains a ROS (Robot Operating System) workspace named `ros_ws`. It is designed as a development environment for building, testing, and running ROS packages, nodes, and projects. Use this workspace to organize your ROS code, dependencies, and configuration files in a structured and maintainable way.

## Table of Contents

- [Workspace Structure](#workspace-structure)
- [Getting Started](#getting-started)
- [Building the Workspace](#building-the-workspace)
- [Running Nodes](#running-nodes)
- [Contributing](#contributing)
- [License](#license)

## Workspace Structure

Typical directory layout:
```
ros_ws/
├── src/             # Source code for ROS packages
├── build/           # Build files (generated)
├── devel/           # Development space (generated)
└── README.md        # This file
```

- Place your ROS packages inside the `src/` directory.

## Getting Started

### Prerequisites

- [ROS](https://www.ros.org/) installed (e.g., ROS Noetic, Melodic, or Humble)
- [catkin tools](https://catkin-tools.readthedocs.io/en/latest/) (`catkin_make`, `catkin build`, or `colcon` for ROS 2)
- Python 3 (for ROS Noetic or later)
- Other dependencies as required by your packages

### Clone the Repository

```bash
git clone https://github.com/nishnarudkar/ros_ws.git
cd ros_ws
```

## Building the Workspace

Navigate to your workspace directory and run:

For ROS 1 (catkin):
```bash
cd ros_ws
catkin_make
# or, with catkin tools (if installed)
catkin build
```

For ROS 2 (colcon):
```bash
cd ros_ws
colcon build
```

## Sourcing the Workspace

Before running any ROS nodes, source your workspace:

For ROS 1:
```bash
source devel/setup.bash
```

For ROS 2:
```bash
source install/setup.bash
```

You can add this source command to your `.bashrc` for convenience.

## Running Nodes

After building and sourcing, you can run your nodes as usual. For example:

```bash
rosrun <package_name> <node_name>
```
or
```bash
roslaunch <package_name> <launch_file.launch>
```

## Contributing

Feel free to fork this repository, open issues, or submit pull requests. Contributions are welcome!

## License

This repository is licensed under the [MIT License](LICENSE), unless otherwise specified.

---

For detailed documentation on ROS, visit the [official ROS documentation](https://docs.ros.org/).

# ROS 2 Development Container for the TurtleBot4 

You want to get started with ROS 2 and the [Turtlebot 4](https://clearpathrobotics.com/turtlebot-4/), however you don't want to upgrade your main OS to Ubuntu 22.04?
This repository contains a setup that uses a Docker container as an isolated environment for ROS 2 development.

## Features

- GPU support 
- Display forwarding
- VS Code configuration
  - ROS 2 approved formatters
  - Pre-defined tasks
  - Debugging setup
- Basic continues integration setup

## Credits

This repository is based on public template from Allison Thackston for a [generic ROS 2 Dev-Container setup](https://github.com/athackst/vscode_ros2_workspace). 

## Set Up

1. Install [Docker](https://docs.docker.com/get-docker/) and [VS Code](https://code.visualstudio.com/download)
2. Install the VS Code [Dev-Containers Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers).
3. If you have a Nvidia GPU, install the [NVIDIA Container Toolkit](https://github.com/NVIDIA/nvidia-container-toolkit) to get GPU acceleration inside the container. Instructions can be found [here](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/install-guide.html#setting-up-nvidia-container-toolkit).
4. Open VS Code press `F1` and use `Dev Containers: Open Folder in Container`. Or use the pop up in the lower right corner.

## Note

- The Docker image is quite larage (around 7.5GB), keep that in mind when deleting, downloading or rebuilding the image.
- **The Container has evelated privileges for performing networking administration**. This gives the container control over the hosts network stack.

## TODOs

- [ ] Provide setup scripts for the discovery server setup.
- [ ] Does WSL work?

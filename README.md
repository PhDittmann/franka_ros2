# ROS 2 integration for Franka Emika research robots

This repository is a fork of [frankaemika/franka_ros2](https://github.com/frankaemika/franka_ros2), because support for Franka Emika Robot (FER) was stopped end of 2023.

```shell
mkdir ~/ros2_ws && cd ~/ros2_ws
git clone --recursive https://github.com/frankaemika/libfranka.git -b 0.9.2 src/libfranka
git clone https://github.com/PhDittmann/franka_ros2.git -b fer src/franka_ros2
colcon build --packages-up-to libfranka
source install/setup.bash
colcon build
```

See the [Franka Control Interface (FCI) documentation][fci-docs] for more information.

## License

All packages of `franka_ros2` are licensed under the [Apache 2.0 license][apache-2.0].

[apache-2.0]: https://www.apache.org/licenses/LICENSE-2.0.html

[fci-docs]: https://frankaemika.github.io/docs

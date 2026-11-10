# Rui Zhou · 周瑞

I build robotics applications on **ROS 2, embedded Linux, Jetson, and ESP32**. I focus on making demos reproducible: documenting the setup, checking results, and making hardware and software failures easier to isolate.

机器人应用与嵌入式开发：板端部署、软硬件联调、案例复现与排障。

## Selected projects

### 1. reBot Arm B601-RS — simulation and MoveIt 2 integration

Reproduced the upstream MuJoCo WASM demo for TCP inverse kinematics, gripper control, and pick-and-place. In a separate ROS 2 Humble setup, I adapted the launch configuration for OMPL and ros2_control virtual hardware. **All six segments of the rectangle demo completed in simulation.** No physical-arm testing has been completed.

**Quick start:** For the browser demo, use the [upstream simulator](https://yang-ci.github.io/ReBot_Arm_DigitalTwin_RS/). For ROS 2, follow the **simulation** section of the [Seeed B601-RS integration guide](https://wiki.seeedstudio.com/rebot_arm_b601_rs_ros2_integration/) and run the draw-square demo. Check that the virtual controllers are active before sending a goal. If planning fails, start with the joint-state feedback, the target TCP pose, and joint limits. The ROS 2 simulation does not require CAN hardware.

### 2. CyberDog 2 — from Gazebo to real hardware

Reused ROS 2 perception and task logic from Gazebo 11, adapted LCM gait commands, and used motion progress and pose feedback to check whether the robot reached its target. The real-hardware footage is from **pre-competition integration testing**.

[Gazebo demo](https://www.bilibili.com/video/BV1HJnp6nEMM/) · [Real-hardware demo](https://www.bilibili.com/video/BV11XeCzvEQX/)

### 3. OmniCart — retail assistant robot

Led software integration for a differential-drive robot: **Jetson Xavier NX** ran ROS 2/Nav2, a custom-trained YOLOv8 product detector, and a Qt interface; **ESP32-S3** handled the drivetrain through micro-ROS. Integrated UWB following and closed-loop wheel-speed control.

[Project demo](https://www.bilibili.com/video/BV1xZ3c6kEAq/)

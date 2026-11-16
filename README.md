<div align="center">

<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&pause=1200&color=F7B93E&center=true&vCenter=true&random=false&width=760&v=3&lines=Hello+World!;I+am+Rui+Zhou;ROS+2+%C2%B7+Embedded+Linux+%C2%B7+Robotics;Reproducible+demos+%C2%B7+Hardware-software+integration" alt="Typing SVG" />
</a>

<h3>👋 你好，我是周瑞</h3>

<p>
  <em>专注机器人应用与嵌入式开发：ROS 2、板端部署、软硬件联调、案例复现与排障。</em>
</p>

</div>

---

## 🧰 技术栈

<div align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=python,cpp,c,linux,ubuntu,docker,git,github,cmake,raspberrypi,arduino,vscode&theme=light" alt="skills" />
  </a>
</div>

---

## 📊 GitHub 数据

<div align="center">

![streak](https://streak-stats.demolab.com/?user=newer888&theme=transparent&hide_border=true)

<a href="https://github.com/newer888?tab=followers">
  <img src="https://img.shields.io/github/followers/newer888?label=Followers&style=for-the-badge&labelColor=343A46&color=23272F" alt="Followers" />
</a>
<a href="https://github.com/newer888?tab=repositories">
  <img src="https://img.shields.io/github/stars/newer888?label=Stars&style=for-the-badge&labelColor=343A46&color=F7B93E" alt="Stars" />
</a>

</div>

---

## 🐍 贡献贪吃蛇

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/newer888/newer888/output/snake-dark.svg" />
  <img src="https://raw.githubusercontent.com/newer888/newer888/output/snake.svg" alt="contribution snake" />
</picture>

---

## 🚀 代表项目

### 1. reBot Arm B601-RS — simulation and MoveIt 2 integration

Reproduced the upstream MuJoCo WASM demo for TCP inverse kinematics, gripper control, and pick-and-place. In a separate ROS 2 Humble setup, I adapted the launch configuration for OMPL and ros2_control virtual hardware. **All six segments of the rectangle demo completed in simulation.** No physical-arm testing has been completed.

**Quick start:** For the browser demo, use the [upstream simulator](https://yang-ci.github.io/ReBot_Arm_DigitalTwin_RS/). For ROS 2, follow the **simulation** section of the [Seeed B601-RS integration guide](https://wiki.seeedstudio.com/rebot_arm_b601_rs_ros2_integration/) and run the draw-square demo. Check that the virtual controllers are active before sending a goal. If planning fails, start with the joint-state feedback, the target TCP pose, and joint limits. The ROS 2 simulation does not require CAN hardware.

### 2. CyberDog 2 — from Gazebo to real hardware

Reused ROS 2 perception and task logic from Gazebo 11, adapted LCM gait commands, and used motion progress and pose feedback to check whether the robot reached its target. The real-hardware footage is from **pre-competition integration testing**.

[Gazebo demo](https://www.bilibili.com/video/BV1HJnp6nEMM/) · [Real-hardware demo](https://www.bilibili.com/video/BV11XeCzvEQX/)

### 3. OmniCart — retail assistant robot

Led software integration for a differential-drive robot: **Jetson Xavier NX** ran ROS 2/Nav2, a custom-trained YOLOv8 product detector, and a Qt interface; **ESP32-S3** handled the drivetrain through micro-ROS. Integrated UWB following and closed-loop wheel-speed control.

[Project demo](https://www.bilibili.com/video/BV1xZ3c6kEAq/)

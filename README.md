# 嵌入式开发项目工程索引

本仓库用于汇总、索引和存放嵌入式开发相关项目工程。各项目可通过独立目录、Git 子模块或外部仓库链接进行管理，便于快速定位、维护与协作。

## 项目列表

### 1. 基于 NVIDIA Jetson 的双足足球机器人

#### C++
- **项目介绍**：该机器人全身18自由度，舵机作为执行器，IMU、工业相机作为感知部件，具有行走、特殊动作、视觉、定位和无线通信功能，整个系统用有限状态机进行控制; 代码在NVIDIA Jetson TX上运行，操作系统为Ubuntu 18.04
- **工程链接**：https://github.com/yizecao2005/robocup_kidsize_seu_2025-2026

#### ROS2
- **项目介绍**：基于原本程序，迁移到ROS2架构，并更换IMU、电路板、相机和视觉算法代码；在NVIDIA Jetson Nano NX 8GB上运行，操作系统为Ubuntu 22.04
- **工程链接**：https://github.com/yizecao2005/robocup_kidsize_seu_2026_ROS2

### 2. 基于 MCU 的定点巡航、自主绕杆与地面目标检测无人机
- **项目介绍**：设计了一个无人机与地面站的协同系统，无人机可以完成自主巡航、绕杆飞行、目标检测、扫描二维码等一系列任务。
- **工程链接**：https://github.com/yizecao2005/Drone_MCU

### 3. 基于 FreeRTOS 与 PID 控制的多任务循迹智能车
- **项目介绍**：竞赛期间主控使用NXP MCU，实现传感器采集、PID运动控制循迹与通信功能；后基于STM32和FreeRTOS进行升级
- **工程链接**：https://github.com/yizecao2005/freertos-pid-car

## 快速索引

| 序号 | 项目名称 | 版本/说明 | 工程链接 |
| --- | --- | --- | --- |
| 1 | 基于 NVIDIA Jetson 的双足足球机器人 | C++版 | https://github.com/yizecao2005/robocup_kidsize_seu_2025-2026 |
| 1 | 基于 NVIDIA Jetson 的双足足球机器人 | ROS2版 | https://github.com/yizecao2005/robocup_kidsize_seu_2026_ROS2 |
| 2 | 基于 MCU 的定点巡航、自主绕杆与地面目标检测无人机 | - | https://github.com/yizecao2005/Drone_MCU |
| 3 | 基于 FreeRTOS 与 PID 控制的多任务循迹智能车 | - | https://github.com/yizecao2005/freertos-pid-car |

## 仓库说明

- 本仓库作为嵌入式开发项目的工程存放位置与索引入口。
- 具体源码、文档、硬件设计、调试记录等内容，请进入对应工程链接查看。
- 新增项目时，请同步更新“项目列表”和“快速索引”部分。
- 若项目以子目录形式存放，建议保持目录名清晰、统一，并在本 README 中登记说明。

## 目录结构建议

```text
.
├── README.md
├── jetson-bipedal-soccer-robot/
├── jetson-bipedal-soccer-robot-upgrade/
├── mcu-uav-waypoint-obstacle-detection/
└── freertos-pid-line-following-car/
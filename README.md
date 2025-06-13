# CMW500RemoteControl
Remote control program for Rohde &amp; Schwarz CMW 500 wideband radio communication tester
-----------------------------------------------------------------------------------------------

## Introduction

This program provides a graphical user interface (GUI) for remotely controlling the Rohde & Schwarz CMW500 Bluetooth tester. It supports the following features:

- Remote connection via VISA protocol  
- Query instrument identification (*IDN?)  
- Configure Bluetooth measurement parameters  
- Start and stop continuous Bluetooth measurement  
- Retrieve and save screenshots from the instrument (PNG format)  
- Real-time log output in GUI  

---

## Requirements

- Python 3.10+
- [NI-VISA](https://www.ni.com/visa/)
- Install the following Python packages:

```bash
pip install pyvisa pyvisa-py
```

---

## Usage

1. Launch the program and enter the instrument's IP address or select a VISA address from the dropdown;
2. Click **Query Device Info** to verify the connection;
3. Click **Set Parameters** to configure Bluetooth settings such as channel, frequency, power, PHY, etc.;
4. Click **Start Measurement** to begin continuous evaluation;
5. To stop measurement, click **Stop Measurement**;
6. Click **Screenshot** to save the current screen as a PNG file in the `screenshots/` folder;
7. All responses and errors will be shown in the log panel below.

---

## File Structure

```
CMW500RemoteControl/
├── CMW500RemoteControl.py   # Main program
├── screenshots/             # Folder where screenshots are saved
└── README.md                # This file
```

---

## Notes

- Ensure NI-VISA is installed and properly configured;
- Some older firmware versions of CMW500 may not support screenshot commands;
- This program is intended for testing and experimental use only.


---


# 🈶 Rohde & Schwarz CMW500远程控制图形界面程序

## 简介

本程序为 Rohde & Schwarz CMW500 蓝牙测试仪设计，提供图形化用户界面（GUI），实现以下功能：

- 通过 VISA 协议远程连接设备  
- 查询仪器型号信息（*IDN?）  
- 设置 Bluetooth 测量参数  
- 启动和停止连续测量  
- 获取并保存仪表截图（PNG 格式）  
- 实时日志输出  

---

## 环境要求

- Python 3.10+
- [NI-VISA](https://www.ni.com/visa/)
- 安装以下 Python 库：

```bash
pip install pyvisa pyvisa-py
```

---

## 使用方法

1. 启动程序后，输入仪器的 IP 地址或手动从下拉菜单选择 VISA 地址；
2. 点击 **读取仪表信息** 验证连接；
3. 点击 **设置参数** 配置 Bluetooth 测试通道、频率、功率、PHY 等参数；
4. 点击 **开始测量** 进行连续评估；
5. 如需停止测量，可点击 **停止测量**；
6. 点击 **仪表截图** 可保存当前屏幕截图为 PNG 文件至 `screenshots/` 文件夹中；
7. 所有响应和错误信息均会实时显示在下方日志栏中。

---

## 文件结构

```
CMW500RemoteControl/
├── CMW500RemoteControl.py   # 主程序
├── screenshots/             # 截图自动保存目录（自动生成）
└── README.md                # 本说明文件
```

---

## 注意事项

- 请确保运行环境中已经安装并配置好 NI-VISA 驱动；
- 截图命令在部分旧型号或固件版本的 CMW500 中可能不受支持；
- 本程序为测试与实验用途开发，请勿用于正式认证流程。

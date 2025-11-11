🖥️ Design and Verification of VGA Controller

A fully functional VGA controller implemented in SystemVerilog, designed to generate synchronized horizontal and vertical timing signals for 640×480 @ 60 Hz display.
Includes RGB color generation, video enable logic, and a testbench for simulation.
Ideal for FPGA-based display applications and digital design learning.

🧭 Overview

This project implements a VGA display controller with color modulation and timing synchronization.
The controller divides the display area into visible and non-visible regions and assigns RGB values dynamically in short intervals to visualize timing behavior.

Additionally, a baud rate generator provides a stable timing pulse that can be used to control the update rate for RGB signals or external synchronization interfaces.


⚙️ Features

Supports 640×480 @ 60 Hz VGA timing standard

Baud generator for fine-grained timing or serial synchronization

Generates HSYNC and VSYNC pulses precisely per VGA standards

Implements active video region control (video_on)

Dynamic RGB pattern output for visual testing and waveform verification

Clean and modular SystemVerilog structure

Fully verified with ModelSim, Vivado, and GTKWave


📊 VGA Timing Parameters (640×480 @ 60 Hz)

| **Signal** | **Visible** | **Front Porch** | **Sync Pulse** | **Back Porch** | **Total** |
| ---------- | ----------- | --------------- | -------------- | -------------- | --------- |
| Horizontal | 640         | 16              | 96             | 48             | 800       |
| Vertical   | 480         | 10              | 2              | 33             | 525       |


🌈 RGB Pattern Behavior

The RGB signal changes automatically at short time intervals to demonstrate color output.

The color cycle includes:

Red → Green → Blue → Cyan → Magenta → Yellow → White

RGB updates are synchronized with the baud generator output for smooth transitions and timing accuracy.

👨‍💻 Author

Niranjan P
📍 Chennai, India
📧 niranjan1872005@gmail.com

🔗 GitHub: Niranjan-P-1872005

🎓 Electronics and Communication Engineering | Digital Design Enthusiast

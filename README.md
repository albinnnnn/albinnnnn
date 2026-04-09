# Albin Jojo

3rd year B.Tech — Electronics & Computer Engineering, Saintgits College of Engineering · KTU  
I work at the hardware-software boundary — edge ML deployments, embedded firmware, and computer vision systems. Most of my work ends up running on real hardware under real constraints.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/albinjojo)
[![Email](https://img.shields.io/badge/albinjojo4@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:albinjojo4@gmail.com)

---

## Projects

### [Plan Disease Detection](https://github.com/albinnnnn/leaf-disease-detector)
`Python` `PyTorch` `YOLOv8` `ONNX Runtime` `Raspberry Pi` `OpenCV` `NumPy`

Two-stage pipeline: a YOLOv8s leaf detector crops the region of interest, which is then passed to a MobileNetV3-Large classifier trained across 10 disease classes on ~33K image crops. Trained with WeightedRandomSampler to handle class imbalance and progressive backbone unfreezing.

Deployed fully offline as FP32 ONNX on Raspberry Pi 4B with Pi Camera v2 — ~600 ms per-frame inference on CPU, no cloud dependency. Achieved a weighted F1 of ~0.93 across all classes.

[View Project](https://github.com/albinnnnn/leaf-disease-detector)


---

### [RFID Attendance System](https://github.com/albinnnnn/edge-based-rfid-attendance-system) — Distributed IoT Attendance Tracking
`C++` `ESP32` `HTTP` `Google Apps Script` `SPIFFS`

Two RFID end nodes read RC522 card UIDs and forward them over HTTP to a central ESP32 edge node, which validates access and logs attendance to Google Sheets in real time. SPIFFS-backed offline queuing ensures no records are lost during connectivity outages — logs sync automatically on reconnect.

[View Project](https://github.com/albinnnnn/edge-based-rfid-attendance-system)

---

### [Smart AI Glasses](https://github.com/albinnnnn/ai-assisted-smart-glasses) — Assistive OCR Reading Aid
`Python` `EasyOCR` `OpenCV` `pyttsx3` `picamera2` `Raspberry Pi Zero W` `Bluetooth Audio`

Fully offline OCR-to-speech wearable on Raspberry Pi Zero W (512 MB RAM). A capacitive touch sensor triggers capture — hold to read text, tap to pause. Audio output via Bluetooth earbuds or wired speaker, no display or cloud dependency. Tuned for ~2–3 s end-to-end latency per capture under severe memory constraints.

[View Project](https://github.com/albinnnnn/ai-assisted-smart-glasses)

---

### [verilog-uart-fsm](https://github.com/albinnnnn/verilog-uart-fsm) — UART Implementation in Verilog
`Verilog` `Icarus Verilog` `GTKWave`

Full UART core from scratch: parameterised baud rate generator (50 MHz → 9600 baud), FSM-based TX/RX with 16× oversampling for mid-bit sampling and glitch rejection. Four-module design: `uart_top`, `baud_rate_generator`, `uart_tx`, `uart_rx`. Verified via loopback simulation — 3/3 test bytes (`0xA5`, `0x3C`, `0xFF`) passed across a 5.2 ms simulation at 1 ps resolution.

[View Project](https://github.com/albinnnnn/verilog-uart-fsm)

---

## Tech

**Languages**  
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![Verilog](https://img.shields.io/badge/Verilog-000000?style=flat-square&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**ML / Computer Vision**  
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![ONNX](https://img.shields.io/badge/ONNX-005CED?style=flat-square&logo=onnx&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)

**Embedded / IoT**  
![ESP32](https://img.shields.io/badge/ESP32-000000?style=flat-square&logo=espressif&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-C51A4A?style=flat-square&logo=raspberry-pi&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat-square&logo=arduino&logoColor=white)
![MQTT](https://img.shields.io/badge/MQTT-660066?style=flat-square&logo=eclipse-mosquitto&logoColor=white)
![PlatformIO](https://img.shields.io/badge/PlatformIO-F5822A?style=flat-square&logo=platformio&logoColor=white)

**Tools**  
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=flat-square&logo=latex&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![KiCad](https://img.shields.io/badge/KiCad-314CB0?style=flat-square&logo=kicad&logoColor=white)

---


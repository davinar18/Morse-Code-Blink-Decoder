# 👁️ Morse Code Eye Blink Sensor  
A real-time communication system that translates eye blinks into Morse code using computer vision and FPGA-based decoding.

> Co-created by Davina Rajendran and Riana Malhotra

## 📌 Overview  
This project enables users with limited motor abilities to communicate by blinking. Using a desktop camera and OpenCV, eye blinks are detected and classified into short (dot) or long (dash) durations. These are then transmitted via serial (UART) to an FPGA, where Morse code is decoded and the output is displayed on a VGA monitor.

## ⚙️ Tech Stack  
- **Python (OpenCV)** - For blink detection and classification  
- **Verilog** - For Morse code decoding logic on the FPGA  
- **UART Serial Communication** - For sending blink data to the board  
- **FPGA Platform** - DE1-SoC Board (Cyclone V)  
- **VGA Display** - For outputting the translated message  

## 🧠 Key Features  
- Real-time blink detection and classification using OpenCV  
- Serial communication between PC and FPGA  
- Morse code decoder written in Verilog  
- VGA text display of the decoded message  
- Support for backspace and live letter composition  

## 🖥️ System Flow  
- User blinks → Webcam captures frames  
- OpenCV tracks eye closure duration  
- Classified as dot or dash and sent via UART  
- Verilog module on FPGA decodes the stream  
- Output displayed as characters on VGA screen  

## 🔬 Why I Built This  
I wanted to explore assistive communication technologies while combining my experience with computer vision and Verilog. This project also helped me improve my understanding of serial communication and real-time input processing on FPGAs.

## 📷 Demo  
*Coming soon* – planning to upload a short demo GIF or video walkthrough.

## 🛠️ How to Run  
Since this was created as part of a course project, I’m unable to publicly share the source code or Verilog files.

That said, here’s an outline of how the system was set up:

1. Blink detection was implemented in Python using OpenCV  
2. Classified blink data (dots and dashes) was sent via UART to the FPGA  
3. The FPGA decoded Morse sequences using Verilog and outputted characters to a VGA screen   

## 📄 Future Improvements  
- Add support for full words and sentence building  
- Add sound output for accessibility  

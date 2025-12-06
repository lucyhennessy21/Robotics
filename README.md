**🤖 WiFi-Powered Robot — Final Project (Arduino UNO R4 WiFi)**
**By: Lucy Hennessy & TJ Laryea**

**📌 Overview**

This project is a WiFi-controlled robot built using the Arduino UNO R4 WiFi, an ultrasonic sensor, and a custom browser-based control interface. The robot responds to directional commands (Up, Down, Left, Right) and includes smart obstacle detection that stops the robot and displays a warning on the LED matrix. Once it’s safe, the robot can resume movement. (See Final Report PDF)

**✨ Features**

- 🌐 WiFi remote control via a web browser

- 🔼🔽⬅️➡️ Directional movement controls

- 📏 Ultrasonic obstacle detection (< 15 cm = stop)

- ⚠️ LED matrix warning circle display

- ▶️ Auto-resume logic after obstacles are cleared

- 🎨 Custom HTML/CSS interface in Kent State colors

- 🛠 Real-time serial output for debugging

**🔧 Hardware Used**

- Arduino UNO R4 WiFi

- Ultrasonic Sensor (HC-SR04)

- Dual Motor Driver

- DC Motors + Wheels

- LED Matrix

- Breadboard + Jumper Wires

- Battery Pack

**💻 Code Structure**

The Arduino C++ program includes:

- 🚗 Motor control functions: forward, backward, turning, stopping, resuming

- 🌐 WiFi server that handles incoming browser commands

- 📡 Continuous distance measurement + safety logic

- 💡 LED matrix bitmap display for warnings

- 🖥 Built-in HTML/CSS page served from the Arduino

The web page includes large buttons, hover effects, and a clean layout compatible with phones and laptops.

**🧪 Testing & Debugging**

Throughout development, we solved several issues:

- 🔄 Motors spinning in incorrect directions

- 🔌 Missing or incorrect serial port connections

- 📶 WiFi failing to connect consistently

- ❌ Ultrasonic sensor returning 0 or -1 due to wiring issues

- 🛑 Robot not resuming after stopping

These were fixed through step-by-step testing, rewiring, adjusting motor logic, resetting WiFi, and using Serial Monitor to verify sensor values and movement behavior.

**🕹 IP Control Page Design**

The control page uses a simple, game-style directional layout.

- 🎮 Large, tap-friendly buttons

- 💙💛 Kent State color theme (blue & gold)

- ✨ Hover and click animations

- 📱 Fully responsive on mobile and desktop

- 🔤 No emojis to ensure Arduino compatibility

**🧩 Team Reflection**

Most challenging part:

- Getting the robot to stop and later resume correctly after obstacle detection.

Division of work:

- One teammate focused on wiring, hardware, and TinkerCAD.

- The other focused on coding, WiFi setup, and HTML interface.

What we learned about debugging:

- Small mistakes (like reversed wires or bad ports) cause big issues.

- Serial Monitor is essential for diagnosing sensor values and behavior.

If we had more time, we would add:

- 🤖 Full autonomous navigation

- 📡 More sensors for 360° detection

- ⚡ Adjustable speed control

Real-world connection:
This project models real systems used in delivery robots, warehouse robots, and smart home devices that combine remote control with sensor-based safety.

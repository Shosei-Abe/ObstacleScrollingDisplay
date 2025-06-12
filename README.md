# Arduino Scrolling Text Display with Button Control 🧠🔲

This is a simple and interactive scrolling text display system built with an Arduino Uno and an 8x8 LED matrix. The system allows switching between multiple messages using buttons, with smooth scrolling implemented manually.

## 🎯 Features

- Scrolling text across an 8x8 LED matrix
- Button-controlled message switching (Next / Previous)
- Custom font rendering (A–Z and space)
- Debounce logic for stable input
- Real-time visual output using Wokwi or real hardware

---

## 🛠 Components Used

| Component             | Quantity | Notes                                 |
|----------------------|----------|----------------------------------------|
| Arduino Uno          | 1        | Main microcontroller                   |
| 8x8 LED Matrix (1088BS) | 1      | Direct row/column wiring, not MAX7219 |
| Push Buttons         | 2        | For switching messages                 |
| Resistors (10kΩ)     | 8        | For pull-down                         |
| Jumper Wires         | Many     | Connections                            |
| Breadboard           | 1        | Circuit setup                          |

---

## 🔌 Arduino Pin Layout

| Function            | Arduino Pin |
|---------------------|-------------|
| LED Matrix Rows     | D2 to D9    |
| LED Matrix Columns  | D10 to D13, A0 to A3 |
| Next Button         | A4          |
| Previous Button     | A5          |

---

## 🔍 How It Works

1. On boot, a default message begins scrolling.
2. Press the **Next** button to display the next message.
3. Press the **Previous** button to go back.
4. Messages scroll one column at a time using custom font rendering.
5. Debounce logic ensures stable button behavior.

---

## 📽 Demo Video

[Click to watch the demo](./assets/video.mp4)  
<img src="./assets/photo.jpeg" width="400"/>

---

## 📷 Circuit Diagram

![Circuit Diagram](./assets/circuit_diagram.png)

---

## 🧪 Online Simulation (Wokwi)

Try it out online:  
👉 [Wokwi Simulation](https://wokwi.com/projects/432503004912552961)

---

## 📁 Source Code

See `robot_code.ino` in this repository.  
The sketch includes scrolling logic, font mapping, button handling, and custom rendering functions.

---

## 🧠 Author

Shosei Abe – [GitHub](https://github.com/Shosei-Abe)

---

## 📜 License

This project is open-source and available under the MIT License.

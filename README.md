# Project-Evanesco
"An interactive Harry Potter-inspired invisibility cloak application using Python and OpenCV for real-time color masking."

## 🧙‍♂️ Project Introduction: The Cloak of Invisibility (But with Code!)

Have you ever wanted to sneak around Hogwarts without Filch catching you? Say less. 

This project is a super fun, interactive Computer Vision application that brings Harry Potter's legendary **"Invisibility Cloak"** straight into the Muggle world! Built using **Python** and **OpenCV**, the system works like pure techno-magic: it captures your empty room first, then tracks a specific color (like a red blanket) in real-time, and instantly cuts-and-pastes the background over it. 

Boom! You get a seamless, mind-bending visual illusion of being completely invisible on screen. Mischief managed! 🪄✨
---

## ✨ Features

* **Real-Time Color Detection:** High-accuracy red color segmentation using the HSV color space.
* **Smart Background Capture:** Automatically records a blank background frame during the initial 5-second delay.
* **Auto-Save Recording:** Seamlessly saves your final invisibility effect video as `invisibility_cloak_output.mp4`.

---

## 🚀 How to Run

1. Clone or download this repository to your local machine.
2. Open Terminal and navigate to your project directory:
   ```bash
   cd "OpenCV Project"
    
3. Execute the Python script:
   ```bash
   python3 main.py
4. ⚠️ **Important:** Step out of the camera frame for the first 5 seconds to let the system capture a clean, empty background.
5. Step back into the frame with a solid red cloth, blanket, or jacket.
6. Press `q` on your keyboard to stop the program and automatically save the video.
---

## 📸 Tech Stack

* **Language:** Python 3
* **Libraries:** OpenCV (`cv2`), NumPy
* **Color Space:** HSV (Hue, Saturation, Value)

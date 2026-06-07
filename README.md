# Project-Evanesco
"An interactive Harry Potter-inspired invisibility cloak application using Python and OpenCV for real-time color masking."

## 🧙‍♂️ Project Introduction: The Cloak of Invisibility (But with Code!)

Have you ever wanted to sneak around Hogwarts without Filch catching you? Say less. 

This project is a super fun, interactive Computer Vision application that brings Harry Potter's legendary **"Invisibility Cloak"** straight into the Muggle world! Built using **Python** and **OpenCV**, the system works like pure techno-magic: it captures your empty room first, then tracks a specific color (like a red blanket) in real-time, and instantly cuts-and-pastes the background over it. 

Evanesco! You get a seamless, mind-bending visual illusion of being completely invisible on screen. Mischief managed! 🪄✨
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
   cd "Invisibility-Cloak-Project"
    
3. Execute the Python script:
   ```bash
   python3 main.py
4. ⚠️ **Important:** Step out of the camera frame for the first 5 seconds to let the system capture a clean, empty background.
5. Step back into the frame with a solid red cloth, blanket, or jacket.
6. Press `q` on your keyboard to stop the program and automatically save the video.
---
## ⚙️ How it Works (Under the Hood)

The project utilizes fundamental image processing and color segmentation techniques:

* **Background Capture:** The script captures multiple frames at the start to store a steady image of the room without any object.
* **Color Space Conversion:** It converts the live video frames from standard BGR to **HSV (Hue, Saturation, Value)** space, which allows for more stable and robust color detection under varying light conditions.
* **Mask Generation:** It targets the Red color spectrum by defining lower and upper boundaries. A binary mask is created where the red areas are separated from the rest of the frame.
* **Morphological Operations:** Functions like `cv2.morphologyEx` are applied to the mask to filter out minor background noise and smooth out the edges of the cloak.
* **Image Blending:** Using bitwise operations, the live frame (excluding the red cloak) and the stored background frame (only where the red cloak is) are combined to generate the final visual illusion.
* **Video Recording:** The final output frames are written in real-time to a file named `invisibility_cloak_output.mp4`.
---
## 📸 Tech Stack

* **Language:** Python 3
* **Libraries:** OpenCV (`cv2`), NumPy
* **Color Space:** HSV (Hue, Saturation, Value)

## 📜 Acknowledgments

This project is inspired by open-source **Invisibility Cloak** projects available on GitHub. 

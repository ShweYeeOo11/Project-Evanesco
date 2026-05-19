# Project-Evanesco
"An interactive Harry Potter-inspired invisibility cloak application using Python and OpenCV for real-time color masking."

## Project Introduction
This project is an interactive Computer Vision application inspired by the "Invisibility Cloak" from Harry Potter. Built using Python and OpenCV, the core system captures the background environment first, then detects a specific color in real-time and replaces it with the pre-captured background. This creates a seamless visual illusion of being completely invisible on screen.

The primary goal of this project is to explore fundamental image processing techniques and color space manipulation (HSV).

---

## Technical Capabilities and Features
"The project is structured to easily accommodate the following interactive features:"

* **Color-Based Invisibility:** The core functionality that utilizes real-time HSV color thresholding to segment the cloak and blend it with the background.
* **Dynamic Background Swapping:** The system can accommodate swapping the hidden area with alternative digital environments or custom images, rather than being limited to the empty room background.
* **Multi-Color Detection:** The masking pipeline has the capacity to handle multiple color profiles simultaneously, enabling multi-user interaction with different colored cloaks.

---

## Tech Stack
* **Language:** Python
* **Core Libraries:** OpenCV, NumPy

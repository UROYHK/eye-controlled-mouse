# eye-controlled-mouse

imagined controlling your computer with just your eyes. This project brings that idea to life. Using a webcam, MediaPipe and Python with this the user can now move your mouse pointer using your eyes and even click by blinking  there is no need for hands.

-->What It Does
*Move the Cursor: Your eye movement controls the mouse.
*Click with a Blink: A simple blink of your left eye triggers a mouse click.
*Real-time Tracking: Powered by MediaPipe FaceMesh for accurate facial landmark detection.
*Hands-Free Control: Ideal for accessibility solutions or just cool tech demos.

-->How It Works
*Webcam Input: The program captures your face using OpenCV.
*FaceMesh Detection: MediaPipe detects 468 facial landmarks in real-time.
*Eye Tracking: It monitors landmarks around your right eye to guide the mouse.
*Blink Detection: It watches your left eye; when you blink (based on landmark distance), it simulates a mouse click.
*Mouse Control: PyAutoGUI moves your system cursor and handles the clicks.

 -->What You Need
Make sure you have Python installed, then run:
bash
Copy
Edit
pip install opencv-python mediapipe pyautogui

-->How to Run
*Save the code as eye_mouse.py.
*Open your terminal and run:
bash
Copy
Edit
python eye_mouse.py
Look into the webcam.
Move your eyes to move the cursor.
Blink your left eye to click.
Make sure you’re in a well-lit environment and facing the webcam.

-->Tech Behind the Scenes
*Library	Purpose:
OpenCV	Video capture and display
MediaPipe	Face landmark detection
PyAutoGUI	Simulating mouse movement and clicks

--> Notes
Eye tracking might vary based on lighting and webcam quality.
If clicks are too sensitive, tweak the blink threshold (0.004) in the code.


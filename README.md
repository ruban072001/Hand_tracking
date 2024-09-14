**Hand Tracking with OpenCV and Mediapipe**

This project demonstrates real-time hand tracking using OpenCV and Mediapipe in Python. It tracks hand landmarks and provides the option to highlight specific landmarks in the video feed. Additionally, the code calculates and displays the frame-per-second (FPS) to monitor the real-time performance.

**Features**

1.Tracks hands in real-time using a webcam.

2.Detects hand landmarks and draws them on the video frame.

3.Allows specifying which hand landmarks to track (e.g., fingertips).

4.Displays the FPS on the video feed.

5.Easily configurable with parameters like the maximum number of hands to track, detection confidence, and tracking confidence.

**Requirements**

To run this project, you need the following Python libraries:

1.**OpenCV**: For capturing video and handling image operations.

2.**Mediapipe**: For hand tracking and landmark detection.

3.**time**: To calculate and display FPS (frames per second).

**How It Works**

**1. HandTracking Class:**

**Initialization:**

**mode**: Static image mode (default is False for video input).

1.max_hands: Maximum number of hands to detect.

2.detection_confidence: Minimum confidence for hand detection.

3.tracking_confidence: Minimum confidence for hand tracking.

4.find_hands(): Detects hands in the frame and optionally draws hand landmarks using Mediapipe's drawing utilities.

**find_position()**: Identifies specific hand landmark positions (e.g., fingertips) and returns their (x, y) coordinates. Optionally draws circles on the specified landmarks.

**2. run_hand_track() Function:**

1.Captures video from the webcam.

2.Uses the HandTracking class to detect and track hand landmarks in real-time.

3.Displays the FPS on the video frame for performance monitoring.

4.Allows users to quit the program by pressing the q key.

# File System Face Recognition

## Project Overview
This Python application combines face detection techniques with filesystem management to create a real-time facial recognition system. Building directly on my OpenCV projects, it captures live webcam video, detects faces, and identifies individuals by comparing face encodings against stored data. The program displays recognized faces with labeled rectangles showing each person's name, and features on-the-fly enrollment that allows adding new faces without restarting.


Activated by pressing "i", enrollment mode displays a fixed red rectangle at the center of the webcam feed. A Haar cascade algorithm ensures a face is properly framed. Once detected, a three-second countdown allows you to steady your position. The program then pauses to request a name, generates a 128-dimensional face embedding from the captured region of interest, adds the vector and name to in-memory lists, saves the face image to the training directory, and immediately begins recognizing the newly added face without requiring a restart.
## Demo vid
[![Watch the video](https://img.youtube.com/vi/mxXeD08ib00/hqdefault.jpg)](https://youtu.be/mxXeD08ib00)

### [Watch this video on YouTube](https://youtu.be/mxXeD08ib00)

## Date Completed
May 2024

## Languages, Libraries & Frameworks
- **Python**
- **OpenCV** (for computer vision operations)
- **os** (for traversing the filesystem to locate training images and save new enrollments)
- **time** (for measuring countdown delays during the enrollment process)
- **face_recognition** (for generating deep-learning-powered face encodings and performing cosine-based comparisons)
- **Haar Cascade XML** (`haarcascade_frontalface_default.xml` for precise face detection within the enrollment rectangle)

## Lines of Code: 115

## Hardware Components Used
- Webcam
- Laptop

## Challenges Overcome
- Processing high-resolution frames in real time without dropping too many FPS
- Resizing frames for detection, then correctly scaling face coordinates back
- Handling multiple faces in a single frame with proper identification
- Creating a graceful enrollment process that validates image quality
- Balancing system responsiveness with processing demands

## Skills Demonstrated
- Matrix manipulation and working with matrices as datasets in the form of images
- Autoscripting file I/O for training data pipeline
- Real-time computer vision pipeline design and optimization
- Modular function creation for hardware configuration
- Debugging camera settings
- Face-encoding management and matching logic
- Seamless integration of CV libraries into a cohesive Python script
- User interface design for interactive enrollment
- File system management for training data
- Real-time feedback systems (countdown timers, status messages)
- Biometric data handling and processing
- Camera calibration and optimization for facial recognition
- Integration of AI-powered computer vision models
- Implementation of deep learning face embedding techniques
- Machine learning integration for identification tasks
- Performance optimization for real-time applications
- Threshold parameter tuning for accuracy/performance balance
- Managing live video capture with complex processing

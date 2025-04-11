# YOLOv11_Video_Object_Detection


A real-time object detection system using YOLOv11 to identify vehicles (cars, trucks, buses) in video streams.
📝 Description

This project leverages the Ultralytics YOLOv11 model to perform object detection on video frames. It processes each frame, detects vehicles (cars, trucks, buses) with confidence scores, and logs performance metrics such as inference time. The implementation is optimized for Google Colab and integrates with Google Drive for easy file management.
✨ Key Features

    Real-Time Detection: Processes video frames and identifies objects with bounding boxes.

    Confidence Thresholding: Logs detection results with confidence scores (e.g., car: 0.84).

    Performance Metrics: Tracks preprocess, inference, and postprocess times per frame.

    Google Colab Integration: Pre-configured for seamless execution in a Colab environment.

    Drive Mounting: Directly accesses videos stored in Google Drive.

🛠️ Installation

    Dependencies:
    bash
    Copy

    pip install ultralytics

    Google Colab Setup:

        Mount Google Drive to access input videos:
        python
        Copy

        from google.colab import drive
        drive.mount('/content/drive')

🚀 Usage

    Upload Video: Place your video file in Google Drive.

    Update Paths: Modify the video input/output paths in the notebook.

    Run Detection: Execute the notebook cells to process the video.

Sample Output:
plaintext
Copy

Frame 2220: Detected car with confidence 0.43
Frame 2220: Detected truck with confidence 0.43
Speed: 4.5ms preprocess, 116.9ms inference, 0.9ms postprocess per image

📊 Results

    Model: YOLOv11n (pretrained on COCO dataset).

    Input Resolution: 384x640 pixels.

    Average Inference Time: ~120-200ms per frame (varies by hardware).

    Detected Classes: Cars, Trucks, Buses.

🤝 Contributing

Contributions are welcome! Open an issue or submit a PR for improvements.
📜 License

MIT License (see LICENSE for details).
🙏 Acknowledgments

    Ultralytics Team for the YOLOv11 model.

    Google Colab for providing GPU resources.

🛠️ Developed by Natwar Upadhyay 

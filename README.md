Object Detection with YOLOv8

This project demonstrates object detection using the YOLOv8
 model. It can process both images and videos, generating annotated outputs with bounding boxes and labels for detected objects.

📂 Project Structure
├── Object_Detection.ipynb   # Main project file
├── README.md                # Documentation

🚀 Features

Detects objects in images and videos

Uses YOLOv8 pre-trained model (yolov8n.pt)

Generates annotated results with bounding boxes and labels

Saves processed videos as output files

🛠️ Installation

Clone this repository:

git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>


Install dependencies:

pip install ultralytics opencv-python-headless matplotlib pillow

📌 Usage

Provide an image file as input → The model will detect objects and display/save the result.

Provide a video file as input → The model will generate output_detected.mp4 with annotated detections.

🖼️ Example Workflow

Upload image/video

YOLOv8 runs inference

Save annotated results as output

(You can add screenshots or sample outputs here.)

📖 Requirements

Python 3.x

Libraries:

ultralytics

opencv-python-headless

matplotlib

pillow

🤝 Contributing

Contributions are welcome!

Fork this repo

Create a new branch (feature-branch)

Commit your changes

Open a Pull Request

📜 License

This project is licensed under the MIT License - see the LICENSE
 file for details.

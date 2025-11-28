Human Pose Estimation using OpenCV

This project performs Human Pose Estimation using OpenCV’s Deep Neural Network (DNN) module and a TensorFlow pre-trained model.
It includes a Streamlit-based user interface that allows users to upload an image and visualize detected human body keypoints and poses.

📌 Features

✔ Upload image for pose estimation
✔ Automatic keypoint detection using neural network (TensorFlow .pb model)
✔ Skeleton drawing between detected joints
✔ Adjustable confidence threshold slider
✔ Demo image support when no image is uploaded
✔ Simple and interactive web UI built with Streamlit

🧠 Technology Stack
Component	Technology
Backend Pose Estimation	OpenCV DNN
UI Framework	Streamlit
Model Type	TensorFlow Pre-trained Graph (.pb)
Image Processing	Pillow & NumPy
🚀 How to Run the Project
1️⃣ Install Dependencies
pip install streamlit opencv-python pillow numpy

2️⃣ Download Required Model File

Download the TensorFlow model file: graph_opt.pb
(Ensure it is placed in the same folder as estimation_app.py)

This model is needed to detect pose keypoints.

3️⃣ Run the Application
streamlit run estimation_app.py

📂 Project Structure
├── estimation_app.py
├── graph_opt.pb          # TensorFlow pose detection model
├── stand.jpg             # Demo image (optional)
└── README.md

📸 Output Details

Original Image — displayed before processing

Pose Estimated Image — skeleton drawn by connecting detected keypoints

Green lines → Bones

Red dots → Keypoints (joints)

You can control detection sensitivity using the Confidence Threshold Slider.

⚠ Requirements & Notes

Make sure uploaded images have a clear full human body visible.

The model supports 18 major body joints.

Performance depends on system hardware.

🎯 Future Enhancements Suggested

🔹 Support for multiple humans
🔹 Real-time pose estimation via webcam
🔹 Export keypoints to JSON for motion analysis
🔹 Angle and posture correctness detection

🧑‍💻 Author

Human Pose Estimation OpenCV Project
Built for academic & research learning purpose.

# AmoCart.ai 🛒🤖

AmoCart.ai is an AI-powered shopping assistant that detects products in real-time using a camera and automatically adds them to a virtual cart. It leverages YOLOv8 for object detection and a similarity-checking system to enhance checkout automation and customer experience in smart retail environments.

> ⚙️ Built for developers, researchers, and product teams interested in building intelligent cart systems.

---

## 🚀 Features

- 🔍 Real-time product detection using **YOLOv8**
- 🧠 Intelligent product matching using visual similarity
- 📸 Webcam integration for live item capture
- 📦 Product tracking and cart summarization
- 🧪 Tools to test model performance and retrain on new datasets

---

## 🧰 Tech Stack

| Component        | Technology              |
|------------------|--------------------------|
| Object Detection | YOLOv8 (Ultralytics)     |
| Backend          | Python, OpenCV, Flask    |
| AI/ML            | PyTorch, scikit-learn    |
| Image Handling   | NumPy, OpenCV            |

---

## 📁 Folder Structure

.
├── app.py # Entry point of the Flask app
├── train_model.py # Custom YOLOv8 training script
├── image_similarity.py # Computes feature similarity between images
├── yolo_check.py # Quick tests for YOLO detection
├── hower_object.py # Hover detection logic
├── yolov8n.pt # YOLOv8 pre-trained model weights
├── requirement.txt # Python dependencies
├── devlog.md # Development log
└── README.md # Project documentation

yaml
Copy
Edit

---

## 🔧 Installation

```bash
# Clone the repository
git clone https://github.com/Mafiyak7/AmoCart.ai.git
cd AmoCart.ai

# (Optional) Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirement.txt
▶️ Usage
Run the Web App:
bash
Copy
Edit
python app.py
This will start a Flask server and open the interface for scanning products via webcam.

📊 Train Your Own Model
To retrain the YOLOv8 model with a custom dataset:

bash
Copy
Edit
python train_model.py
Make sure your dataset is in YOLOv5/YOLOv8 format with correct directory structure and data.yaml config.

🧠 Run Image Similarity Search
bash
Copy
Edit
python image_similarity.py --query path/to/image.jpg
This compares a given product image with the known dataset and finds the closest match.

✅ Future Improvements
🔁 Add support for barcode detection fallback

📈 Integrate billing system for real-world use

🖼️ Expand product dataset for more accuracy

Here's your updated README.md with a GitHub badges section added and the License section removed, as requested. The badges are placed right after the project title for visibility:


---

🎥 VidSlide AI

   

VidSlide AI is a web application that transforms long YouTube lectures and presentations into clean, downloadable slide decks. Just paste a YouTube link and let the app use advanced machine learning to detect and extract key presentation slides into a .pptx file.

> 🚀 Turn videos into presentations in seconds!




---

📑 Table of Contents

Introduction

Screenshots

Features

Tech Stack

Project Structure

Installation

Usage

Configuration

Examples

Troubleshooting

Contributors



---

🧠 Introduction

Have you ever sat through an hour-long YouTube lecture and just wanted the slides? VidSlide AI does exactly that.

Built with Python and Flask, this web app allows users to paste any YouTube video URL and uses a ResNet50 model to detect stable slide frames, extract them, and generate a PowerPoint file—automatically.


---

🖼 Screenshots

> 💡 Add actual images in the images/ folder and update the links below.



Home Page	Slide Preview Page

	



---

✨ Features

🔗 YouTube Integration – Works with any public YouTube video link.

🧠 Slide Detection – Uses a ResNet50 ML model to find stable slides while ignoring animations/transitions.

🎚 Sensitivity Control – Choose from Low, Normal, or High slide detection sensitivity.

📦 PowerPoint & ZIP Export – Download slides as .pptx or as a .zip of images.

🌐 Web-Based UI – Clean, responsive interface with preview functionality.

🔐 Secure Sessions – Temporary session folders are isolated and auto-deleted after use.

🌗 Dark Mode – Toggle between light and dark themes.



---

🛠 Tech Stack

Backend:

Python

Flask


Machine Learning:

TensorFlow (Keras)

Scikit-learn


Video Processing:

OpenCV

yt-dlp


Presentation Generation:

python-pptx


Frontend:

HTML

CSS

JavaScript



---

📂 Project Structure

VidSlide-AI/
│
├── .gitignore
├── README.md
├── requirements.txt
├── app.py
│
├── static/
│   └── style.css
│
├── templates/
│   ├── index.html
│   └── preview.html
│
└── sessions/           # Temporary session folders (ignored by Git)


---

🧪 Installation

Follow these steps to run the project locally:

1. Clone the Repository

git clone https://github.com/saurabh9835/VidSlide_AI.git
cd VidSlide_AI

2. Create and Activate a Virtual Environment

# Create the environment
python -m venv venv

# Activate on Windows
venv\Scripts\activate

# Activate on macOS/Linux
source venv/bin/activate

3. Install Dependencies

pip install -r requirements.txt

4. Run the Application

python app.py

Then open your browser and go to:
👉 http://127.0.0.1:5000


---

⚙ Configuration

No additional configuration is required. All sessions are created dynamically and cleaned up after use. For deployment or custom configurations, consider:

SESSION_FOLDER path

Model loading/custom ML pipeline

Web server setup (e.g., Gunicorn, Nginx for production)



---

📌 Usage

1. Paste a YouTube video URL.


2. Select sensitivity level (Low, Normal, High).


3. Click "Extract Slides".


4. Preview and download your .pptx or .zip file.




---

💡 Examples

> Coming Soon: GIFs or screenshots showing the slide extraction process.




---

🛠 Troubleshooting

Video Not Downloading?
Ensure the video is public and yt-dlp is installed correctly.

No Slides Detected?
Try lowering the sensitivity or choose a video with more static slides.

Server Crashes?
Check console logs and ensure dependencies (like TensorFlow) are properly installed.



---

👤 Contributors

Author: Saurabh
🔗 LinkedIn – Update This Link


---

Let me know if you'd like the badges customized further (e.g. with CI status, deployment badge, Python version support, etc.).

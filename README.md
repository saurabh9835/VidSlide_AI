🎥 VidSlide AI 🔥
Have you ever watched a long lecture or presentation on YouTube and wished you could just get the slides? VidSlide AI is a web application that does exactly that. By simply pasting a YouTube video link, this tool uses machine learning to intelligently detect and extract key presentation slides, compiling them into a downloadable PowerPoint (.pptx) file.

This project is built with Python and Flask, providing a clean web interface for a powerful backend process.

🖼️ Screenshots
(It's highly recommended to add screenshots of your application here. Create an images folder in your repository and update the paths below.)

Home Page

Slide Preview Page

✨ Features
YouTube Integration: Works with any public YouTube video link.

Advanced Slide Detection: Uses a ResNet50 machine learning model to analyze frames and accurately detect stable slides, ignoring transitions and animations.

Adjustable Sensitivity: Users can choose between "Low," "Normal," or "High" sensitivity to generate fewer or more slides depending on the video's pacing.

PowerPoint & ZIP Export: Generates a ready-to-use .pptx presentation and a .zip archive containing all extracted slide images.

Web-Based Interface: A clean and user-friendly UI with a slide preview page.

Secure Session Management: Each user's request is handled in an isolated session folder, which is automatically cleaned up to save server space.

Dark Mode: Includes a theme toggle for user preference.

🛠️ Tech Stack
Backend: Python, Flask

Machine Learning: TensorFlow (Keras), Scikit-learn

Video Processing: OpenCV, yt-dlp

Presentation Generation: python-pptx

Frontend: HTML, CSS, JavaScript

📂 Project Structure
VidSlide-AI/
│
├── .gitignore          # Specifies files for Git to ignore
├── README.md           # This file
├── requirements.txt    # Python dependencies
├── app.py              # The main Flask application
│
├── static/
│   └── style.css       # All CSS styling
│
├── templates/
│   ├── index.html      # The main landing/upload page
│   └── preview.html    # The page to preview generated slides
│
└── sessions/           # Auto-created for temporary files (ignored by git)
🚀 How to Run Locally
Follow these steps to get the project running on your local machine.

1. Clone the Repository

Bash

git clone https://github.com/saurabh9835/VidSlide_AI.git
cd VidSlide_AI
2. Create and Activate a Virtual Environment
It's recommended to use a virtual environment to manage dependencies.

Bash

# Create the environment
python -m venv venv

# Activate on Windows
venv\Scripts\activate

# Activate on macOS/Linux
source venv/bin/activate
3. Install Dependencies
Install all the required Python libraries from the requirements.txt file.

Bash

pip install -r requirements.txt
4. Run the Application

Bash

python app.py
The application will now be running. Open your web browser and navigate to:
http://12.0.0.1:5000 🎉

👤 Author
Saurabh

GitHub: @saurabh9835

LinkedIn: Your LinkedIn Profile (<- Update this link)

⭐ Please star this repository if you find it helpful!












Tools


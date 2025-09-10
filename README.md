# 📸 Face Recognition Based Attendance System

![attendance](https://img-c.udemycdn.com/course/750x422/5053658_15ce_2.jpg)

An automated **Attendance Management System** powered by **Face Recognition**.  
This project uses **OpenCV** and **MediaPipe** to detect and recognize faces, then marks attendance automatically in a CSV file.

---

## 🚀 Features

- 🔍 **Face Detection** using OpenCV’s Haar Cascade Classifier  
- 🧑‍🤝‍🧑 **Face Recognition** trained on sample images (Barack Obama, Lionel Messi, Sachin Tendulkar)  
- 📊 **Attendance Tracking** with automatic CSV logging  
- ⚡ **Real-time Processing** through camera feed or static images  
- 🛠️ **Customizable** – Extendable to support any dataset of faces  

---

## 🛠️ Dependencies

The project requires the following Python libraries:

- `opencv-python`
- `mediapipe`
- `numpy`
- `pandas`

---

## ⚙️ Installation

Clone this repository and set up the environment:

```bash
# Clone repo
git clone https://github.com/Careless-Caramel/attendance-project.git
cd attendance-project

# (Optional) Create virtual environment
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

> If `requirements.txt` is missing, install manually:
> ```bash
> pip install opencv-python mediapipe numpy pandas
> ```

---

## ▶️ Usage

1. Place your **training images** inside a folder (e.g., `images/`).  
   - Include only the people you want to recognize (e.g., Obama, Messi, Tendulkar).  
2. Run the Jupyter Notebook:  

```bash
jupyter notebook main.ipynb
```

3. Steps inside the notebook:  
   - Convert input image/video to grayscale  
   - Detect faces with `haarcascade_frontalface_default.xml`  
   - Match with known encodings  
   - Mark attendance in `attendance.csv`  

4. The CSV will look like:

| Name             | Time             |
|------------------|------------------|
| Lionel Messi     | 2025-09-10 09:32 |
| Sachin Tendulkar | 2025-09-10 09:34 |

---

## 📂 Project Structure

```bash
attendance-project/
│
├── main.ipynb                   # Core notebook (training + testing + attendance)
├── haarcascade_frontalface_default.xml  # Face detection model
├── images/                      # Training images (face samples)
├── attendance.csv               # Attendance log file (auto-generated)
├── requirements.txt             # Python dependencies
└── README.md                    # Project documentation
```

---

## 🤝 Contributing

Contributions are welcome!  

1. Fork the repo  
2. Create a feature branch (`git checkout -b feature-name`)  
3. Commit changes (`git commit -m 'Added new feature'`)  
4. Push to your fork (`git push origin feature-name`)  
5. Open a Pull Request  

---

## 👩‍💻 About Me

Hi, I'm **Anna** 👋  
I am an **AI Enthusiast** and **Data Science & ML practitioner**.  
Let’s connect and build amazing AI projects together! 🚀  

---

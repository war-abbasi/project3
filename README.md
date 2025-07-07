# 🧠 Streamlit + OpenCV + ML App

<div align="center">

🔍 <strong>Real-Time Image Classification with Streamlit + OpenCV</strong><br>
💡 Powered by MobileNetV2 via <strong>TensorFlow</strong> or <strong>PyTorch</strong><br>
⚙️ Runs fully in a local virtual environment using <a href="https://github.com/astral-sh/uv">uv</a>

</div>

---

## 🚀 Features

* 📸 Upload images or capture frames using webcam (OpenCV)
* 🧠 Real-time image classification with **MobileNetV2**
* 🖼️ Interactive prediction display
* 🎨 Simple yet powerful UI built with **Streamlit**
* ✅ Easy setup in isolated `.venv` via `uv`

---

## 🧰 Tech Stack

![Python](https://img.shields.io/badge/Python-3.12+-blue?logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-Enabled-red?logo=streamlit)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green?logo=opencv)
![PyTorch](https://img.shields.io/badge/PyTorch-Compatible-orange?logo=pytorch)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Optional-yellow?logo=tensorflow)

---

## 🗂️ Project Structure

<details>
<summary>Click to expand</summary>

```bash
Python_Project_2/
├── .venv/                # Virtual environment (managed by uv)
├── main.py               # Streamlit application script
├── 2.png                 # Main screenshot for README
├── 1.png                 # Demo preview image
├── requirements.txt      # Optional requirements list
└── README.md             # Project documentation
```

</details>

---

## 🧑‍💻 Getting Started

### 🔧 Step 1: Clone the repository

```bash
git clone https://github.com/war-abbasi/project3.git
cd project3
```

Or download the ZIP and extract it.

---

### 🔧 Step 2: Initialize virtual environment

```bash
uv init .
```

---

### 🔧 Step 3: Install dependencies

Choose **one** depending on your model preference:

#### ✅ Option A — PyTorch (Recommended, Python 3.13 compatible)

```bash
uv add streamlit opencv-python torch torchvision --link-mode=copy --no-cache
```

#### ⚠️ Option B — TensorFlow (Requires Python ≤ 3.12)

```bash
uv add streamlit opencv-python tensorflow --link-mode=copy --no-cache
```

---

### 🔧 Step 4: Launch the app

```bash
.venv\Scripts\activate  # Windows
# or
source .venv/bin/activate  # Linux/macOS

streamlit run main.py
```

App will open in your browser at:
👉 `http://localhost:8501`

---

## ⚙️ How It Works

1. The **Streamlit UI** handles image upload or webcam input
2. **OpenCV** processes the input image or live frame
3. A **MobileNetV2 model**, loaded via PyTorch or TensorFlow, performs classification
4. Results are rendered in real-time on the interface

---

## 💡 Example Use Cases

| Scenario               | Description                               |
| ---------------------- | ----------------------------------------- |
| 🧍‍♂️ Object Detection | Classify everyday objects from images     |
| 🎥 Webcam Vision       | Live object recognition using camera      |
| 🖼️ OpenCV Filters     | Add filters or transformations (optional) |
| ⚡ Quick Prototyping    | Deploy and test lightweight ML models     |

---

## 🖼️ App Demo

<p align="center">
  <img src="1.png" alt="App Demo Screenshot" width="100%" />
</p>

---

## 🛠 Troubleshooting

| Issue                           | Solution                                                  |
| ------------------------------- | --------------------------------------------------------- |
| `ModuleNotFoundError`           | Install packages with `uv add <package>` inside `.venv`   |
| `.DS_Store: os error 32`        | Use `--link-mode=copy --no-cache` in `uv add` command     |
| TensorFlow fails on Python 3.13 | Use PyTorch or downgrade to Python 3.12                   |
| OneDrive file lock issues       | Move project to a non-OneDrive directory (e.g., `C:\Dev`) |

---

## 📄 License

Licensed under the **MIT License**.
Feel free to use, improve, and share.

---

## 🙏 Acknowledgements

* [Streamlit](https://streamlit.io/)
* [OpenCV](https://opencv.org/)
* [PyTorch](https://pytorch.org/)
* [TensorFlow](https://tensorflow.org/)
* [UV Package Manager](https://github.com/astral-sh/uv)

---

## 👩‍💻 Author

**Wardah Zia Abbasi**
🔗 [GitHub: @war-abbasi](https://github.com/war-abbasi)

---

If you'd like, I can create a custom banner or a badge section for GitHub Actions, Deploy to Streamlit Cloud, etc. Just let me know!

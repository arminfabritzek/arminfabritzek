# Hi, I’m Armin Fabritzek 👋
**Biologist → AI Engineer** building computer‑vision systems for wildlife monitoring.

--- 
<div align="center">
  <!-- row 1 -->
  <img src="https://img.shields.io/badge/Python-0057B8?style=for-the-badge&logo=python&logoColor=FFD700" alt="Python" width="80" style="margin:3px;"/>
  <img src="https://img.shields.io/badge/PyTorch-0057B8?style=for-the-badge&logo=PyTorch&logoColor=FFD700" alt="PyTorch" width="80" style="margin:3px;"/>
  <img src="https://img.shields.io/badge/OpenCV-0057B8?style=for-the-badge&logo=opencv&logoColor=FFD700" alt="OpenCV" width="80" style="margin:3px;"/>
  <img src="https://img.shields.io/badge/YOLO-0057B8?style=for-the-badge&logo=yolo&logoColor=FFD700" alt="YOLO" width="80" style="margin:3px;"/>
  <img src="https://img.shields.io/badge/EfficientNet-0057B8?style=for-the-badge&logo=efficientnet&logoColor=FFD700" alt="EfficientNet" width="80" style="margin:3px;"/>

  <br/>

  <!-- row 2 -->
  <img src="https://img.shields.io/badge/pandas-FFD700?style=for-the-badge&logo=pandas&logoColor=0057B8" alt="pandas" width="80" style="margin:3px;"/>
  <img src="https://img.shields.io/badge/matplotlib-FFD700?style=for-the-badge&logo=matplotlib&logoColor=0057B8" alt="matplotlib" width="80" style="margin:3px;"/>
  <img src="https://img.shields.io/badge/folium-FFD700?style=for-the-badge&logo=leaflet&logoColor=0057B8" alt="folium" width="80" style="margin:3px;"/>
  <img src="https://img.shields.io/badge/geopandas-FFD700?style=for-the-badge&logo=python&logoColor=0057B8" alt="geopandas" width="80" style="margin:3px;"/>
  <img src="https://img.shields.io/badge/FFmpeg-FFD700?style=for-the-badge&logo=ffmpeg&logoColor=0057B8" alt="FFmpeg" width="80" style="margin:3px;"/>
</div>

---

> 🐦 **WatchMyBirds** — real‑time bird detection **and** species classification from webcams & RTSP streams.

[🔗 App](https://github.com/arminfabritzek/WatchMyBirds) · [🧪 Training Pipeline](https://github.com/arminfabritzek/watchmybirds-pipeline) · [🤗 Model on HF](https://huggingface.co/arminfabritzek/WatchMyBirds-Models/tree/main)

---

## 🚀 WatchMyBirds at a glance
- **Realtime** object detection (YOLOv8) + **species classification** (EfficientNet)
- **End‑to‑end pipeline**: data prep → verification → HPO (Optuna/MLflow) → training → ONNX export → Hugging Face upload
- **29 species**, ~10k images; automatic pre‑annotation via GroundingDINO (+ optional SAM)
- **Results**: OD mAP@[.5:.95] = **xx %** · CLS top‑1 = **xx %** (val)
- **Tracking**: MLflow experiments; model registry with “latest” pointers

<a id="watchmybirds-demo"></a>

![WatchMyBirds Demo](https://raw.githubusercontent.com/arminfabritzek/WatchMyBirds/main/assets/birds_1280.gif)

---

## 🔧 Tech I use on this project
Python · PyTorch · Ultralytics YOLO · timm/EfficientNet · OpenCV · Optuna · MLflow · Hugging Face · ONNX


---

## 🚀 Featured Projects
### [WatchMyBirds App](https://github.com/arminfabritzek/WatchMyBirds)  
**WatchMyBirds** is an AI-powered **real-time object detection system** for birdwatching and wildlife monitoring using webcams, IP-cams & RTSP streams. It supports **webcams**, **IP cameras**, and **RTSP streams**, turning any camera into a **smart detection system**.

---

![WatchMyBirds Demo](https://raw.githubusercontent.com/arminfabritzek/WatchMyBirds/main/assets/birds_1280.gif)  

---

### 🐦 WatchMyBirds Pipelines
Fully automated training pipeline using modern tools like PyTorch, Hugging Face (--> Optuna and MLflow). End-to-end data preparation & training pipelines for object detection and species classification.

**🧩 Key Features**

- ✅ Modular and configurable (YAML-based)
- 🧠 State-of-the-art transfer learning (EfficientNet)
- 🔍 Automated hyperparameter tuning with Optuna
- 📈 MLflow tracking for all experiments
- ☁️ Optional Hugging Face model export
- 🧪 Easily extendable to other image classification tasks


**🧭 Features Overview**

**🔎 Zero-Shot Preannotation**

- Uses Grounding DINO (with optional SAM) to preannotate bird bounding boxes.
- Reads metadata CSV, processes images in batches with ensemble prompts.
- Applies NMS, nested-box filtering, and optional SAM refinement.
- Outputs COCO-format annotations back into the CSV.

**🗂️ YOLO Dataset Preparation**

- Reads and filters metadata based on your criteria.
- Generates YOLO-format image and label files.
- Adds augmentation, class balancing, and negative samples.
- Produces ready-to-train dataset with config and split files.

**🚀 YOLO Training Pipeline**

- Manages environment and TensorBoard logging.
- Loads configs and runs training with checkpointing.
- Exports the best weights to ONNX.
- Bundles final training and inference configs automatically.

**🦜 Classification Dataset Preparation**

- Creates square image crops per species.
- Handles train/val/test splitting and class balancing.
- Augments data and outputs organized dataset folders with run settings.

**🎯 EfficientNet Fine-Tuning**

- Sets up mixed-precision training with mixup/cutmix.
- Progressive backbone unfreezing and LR scheduling.
- Tracks metrics via TensorBoard.
- Saves and exports the best weights (PyTorch + ONNX) with full run configs.

---


### 🚀 Interests & Collaboration

🦾 **Autonomous Systems & Robotics**  
🔬 **AI-driven Biodiversity Research**  
🤖 **Multi-Agent Systems & AI**  


---


### 📡 Other Projects
🔬 **PalaeoMapEurope** – A **Python-based visualization tool** mapping human artifacts and vegetation zones in Europe during the Quaternary period.  
📍 Uses **geospatial mapping, radiocarbon dating, and vegetation analysis** to study human-environment interactions.  
📂 [Explore the Repository](https://github.com/arminfabritzek/PalaeoMapEurope)  


---

### 📫 How to Reach Me
- **LinkedIn**: [linkedin.com/in/arminfabritzek](https://www.linkedin.com/in/arminfabritzek)
- **Email**: armin@starmin.de
- **ORCID**: [https://orcid.org/0000-0002-0199-6802](https://orcid.org/0000-0002-0199-6802)

---

### 📊 GitHub Stats
![Meine GitHub-Statistiken](https://github-readme-stats.vercel.app/api?username=arminfabritzek&show_icons=true&theme=radical)
---


<!---
arminfabritzek is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

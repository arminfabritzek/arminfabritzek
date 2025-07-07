# Hi, I’m Armin Fabritzek 👋  
**Biologist • AI researcher • Software developer**  
Biologist turned AI-engineer, building CV pipelines to monitor wildlife in real time.

---
**Tech & Tools:**  
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

## 🚀 Featured Projects
### [WatchMyBirds](https://github.com/arminfabritzek/WatchMyBirds)  
**WatchMyBirds** is an AI-powered **real-time object detection system** for birdwatching and wildlife monitoring using webcams, IP-cams & RTSP streams. It supports **webcams**, **IP cameras**, and **RTSP streams**, turning any camera into a **smart detection system**.

---

![WatchMyBirds Demo](https://raw.githubusercontent.com/arminfabritzek/WatchMyBirds/main/assets/birds_1280.gif)  

---

### WatchMyBirds-Pipelines  
End-to-end data prep & training pipelines for object detection & classification


**[02_preannotate_v0x.py](https://github.com/arminfabritzek/WatchMyBirds-Data/blob/main/02_preannotate_v0x.py)**: Preannotation using Grounding DINO and SAM

Automates zero-shot preannotation of bird bounding boxes: reads the metadata CSV, processes images in batches using Grounding DINO (and optional SAM) with ensemble prompts, applies NMS and nested-box filtering (and SAM refinement if enabled), then writes COCO-format annotations back into the CSV.

**[5_OD_prepare_data_v0x.py](https://github.com/arminfabritzek/WatchMyBirds-Train-YOLO/blob/main/5_OD_prepare_data_v0x.py)**: Dataset split + augmentation for YOLO

Automates preparation and splitting of a YOLO object-detection dataset: reads and filters metadata, generates image and label files, applies augmentation and class balancing, adds negative samples, and outputs the required configuration and split files.

**[6_OD_train_yolo_v0x.py](https://github.com/arminfabritzek/WatchMyBirds-Train-YOLO/blob/main/6_OD_train_yolo_v0x.py)**: YOLO training, TensorBoard & ONNX export

End-to-end YOLO training pipeline: manages environment and TensorBoard, loads configs and data, runs model training, exports the best weights to ONNX, and assembles all training and inference configuration files.

**[7_CLASSI_prepare_data_classify_v0x.py](https://github.com/arminfabritzek/WatchMyBirds-Classifier/blob/main/7_CLASSI_prepare_data_classify_v0x.py)**: Crop & balance for EfficientNet classifier

Automates preparation of a species‐classification dataset: reads and filters metadata, creates and resizes square image crops per species, splits into train/val/test, balances classes via augmentation and downsampling, and outputs the final organized folders with run settings.

**[8_CLASSI_train_efficientnet_v0x.py](https://github.com/arminfabritzek/WatchMyBirds-Classifier/blob/main/8_CLASSI_train_efficientnet_v0x.py)**: Mixed-precision finetuning with Mixup/CutMix 

Fine-tunes an EfficientNet classifier on the prepared dataset: sets up data transforms and loaders, initializes model architecture and hyperparameters, runs mixed-precision training with mixup/cutmix, backbone unfreezing and learning-rate scheduling, logs metrics to TensorBoard, saves and exports the best weights (including ONNX), and records all run settings.

---


### 📡 Other Projects
🔬 **PalaeoMapEurope** – A **Python-based visualization tool** mapping human artifacts and vegetation zones in Europe during the Quaternary period.  
📍 Uses **geospatial mapping, radiocarbon dating, and vegetation analysis** to study human-environment interactions.  
📂 [Explore the Repository](https://github.com/arminfabritzek/PalaeoMapEurope)  

---

### 🚀 Interests & Collaboration
🦾 **Autonomous Systems & Robotics**  
🔬 **AI-driven Biodiversity Research**  
🤖 **Multi-Agent Systems & AI**  

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

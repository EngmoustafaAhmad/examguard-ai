# 📚 Dataset

ExamGuard AI uses multiple public datasets for initial experimentation, model development, and evaluation.

Because ExamGuard involves different Computer Vision tasks, we use both **image-based** and **video-based** datasets.

Our long-term goal is to build a **custom dataset representing Egyptian examination environments**.

---

## 🎯 Dataset Strategy

```text
                    Camera Video
                         │
                         ↓
                   Frame Extraction
                         │
              ┌──────────┴──────────┐
              ↓                     ↓
        Object Detection       Behavior Analysis
              │                     │
        Image Dataset          Video Dataset
              │                     │
              └──────────┬──────────┘
                         ↓
                  Student Tracking
                         ↓
                  Suspicion Scoring
                         ↓
                       Alert

```
# 📚 Dataset


# 🖼️ Image-Based Datasets

Image datasets will mainly be used for **object detection** and initial **behavior detection** experiments.

## 1. CCTV Exam Monitor Dataset

The **CCTV Exam Monitor Dataset** is one of our primary datasets for initial examination-room experiments.

### Dataset Source

[Kaggle – CCTV Exam Monitor Dataset](https://www.kaggle.com/datasets/cctvdataset/cctv-exam-monitor-dataset?resource=download)

### Example Classes / Behaviors

- Correct Posture
- Left Side Movement
- Right Side Movement
- Forward Movement
- Backward Movement
- Standing

### Purpose

This dataset will help us study:

- Examination-room environments
- CCTV camera perspectives
- Student detection
- Student posture
- Basic suspicious movements

---

## 2. ExamCheating MultiV-Based Dataset

An image-based exam-cheating dataset that can be used for additional experimentation with suspicious examination behaviors.

### Dataset Sources

- [Roboflow – ExamCheating MultiV-Based Dataset](https://universe.roboflow.com/classroom-ornbo/exam-cheating-9iz1y-rrfsz-msjrm)
- [Zenodo – ExamCheating MultiV-Based Dataset](https://zenodo.org/records/14606173)

### Purpose

This dataset can be used as supplementary data for:

- Suspicious behavior detection
- Student behavior classification
- Object detection experiments
- Model comparison

---

# 🎥 Video-Based Datasets

Video datasets are important for ExamGuard because many behaviors cannot be understood from a single image.

For example:

```text
Single Frame
     ↓
Student touching ear
     ↓
Not necessarily suspicious

```
### But:
```text
Video Sequence
     ↓
Repeated ear touching
     ↓
Behavior over time
     ↓
More meaningful analysis

```

## 3. ExamCheating MultiV Video-Based Dataset

This dataset provides video-based examination and cheating scenarios.

### Dataset Source

[Kaggle – ExamCheating MultiV Video-Based Dataset](https://www.kaggle.com/datasets/rimmajeed/examcheating-multiv-video-based-dataset)

### Purpose

The video dataset will be investigated for:

- Temporal behavior analysis
- Suspicious movement patterns
- Normal vs. suspicious behavior
- Behavior recognition
- Video-to-frame extraction
- Testing behavior analysis approaches


# 🗂️ Dataset Categories

The final ExamGuard dataset can be divided into three main categories:

```text
Custom Egyptian Exam Dataset
│
├── Object Detection
│   ├── Person
│   ├── Mobile Phone
│   ├── Tablet
│   ├── Earbuds
│   └── Headphones
│
├── Normal Behavior
│   ├── Writing
│   ├── Reading
│   ├── Looking at Paper
│   └── Normal Movement
│
└── Suspicious Behavior
    ├── Looking Around
    ├── Ear Touch
    ├── Talking
    ├── Unusual Movement
    └── Paper Exchange
```

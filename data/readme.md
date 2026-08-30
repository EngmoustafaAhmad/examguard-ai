# 📚 Dataset

ExamGuard AI uses multiple public datasets for initial experimentation, model development, and evaluation.

Because ExamGuard involves different Computer Vision tasks, we use both **image-based** and **video-based** datasets.

Our long-term goal is to build a **custom dataset representing Egyptian examination environments**.

---

## 🎯 Dataset Strategy

```text
                 ExamGuard Dataset
                        │
          ┌─────────────┴─────────────┐
          ↓                           ↓
    Image Datasets              Video Datasets
          │                           │
          ↓                           ↓
 Object / Behavior             Behavior Analysis
    Detection                  & Temporal Patterns
          │                           │
          └─────────────┬─────────────┘
                        ↓
              Custom Egyptian Dataset
                        ↓
                Final AI Model

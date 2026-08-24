# ExamGuard AI 🛡️

> AI & Computer Vision module for the ExamGuard intelligent examination surveillance system.

ExamGuard AI is the Computer Vision and Artificial Intelligence module of the **ExamGuard** project. It analyzes examination-room camera footage to detect suspicious student behaviors and critical objects, track individual students, calculate suspicion scores, and generate alerts for the invigilator.

The system follows a **Human-in-the-Loop** approach:

> **AI detects. Human decides.**

---

## 🎯 Project Objective

The goal of ExamGuard AI is to assist invigilators during examinations by continuously analyzing camera footage and identifying situations that require human attention.

The AI system does **not** make the final decision that a student is cheating.

Instead:

```text
Camera
   ↓
AI Analysis
   ↓
Detection
   ↓
Behavior Analysis
   ↓
Suspicion Score
   ↓
Alert
   ↓
Invigilator Review
   ↓
Final Decision
```


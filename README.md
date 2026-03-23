# 🖐️ Handwritten Recognition (MNIST, EMNIST & OCR)

A deep learning project recognizing handwritten digits, letters, and full words using **CNNs** and **Pre-trained CRNN**.

## 📊 Results at a Glance

| Task | Dataset/Method | Accuracy/Confidence |
| :--- | :--- | :---: |
| **Digits (0-9)** | MNIST (Custom CNN) | **99.03%** |
| **Letters (A-Z)** | EMNIST (Custom CNN) | **93.81%** |
| **Words** | EasyOCR (Pre-trained CRNN) | **~92% Avg** |

> 💡 **Key Win:** Fixed EMNIST rotation issues (`rot90` + `flip`) to boost letter accuracy from <60% to **93.81%**.

## 🛠️ Tech Stack
*   **Core:** TensorFlow 2.x, Keras
*   **OCR Engine:** EasyOCR (CRNN + CTC)
*   **Tools:** OpenCV, Matplotlib, Google Colab (T4 GPU)

## 🚀 Quick Start
1.  **Open** notebooks in Google Colab.
2.  **Mount Drive:** Run the setup cell to save results automatically.
3.  **Run All:** Trains models (digits/letters) or runs OCR on custom images.

## 📁 Project Structure
```text
CodeAlpha_HandwrittenRecognition/
├── notebooks/          # MNIST, EMNIST, and OCR code
├── models/             # Saved .h5 weights (Digits & Letters)
├── images/             # Test images (test1.png - test9.png)
└── results/            # JSON reports, summaries, and plots
```

## 🔮 Future Work
*   Train custom CRNN for handwriting (IAM Dataset).
*   Deploy as a Streamlit web app.
*   Add multi-language support (Arabic, French, etc.).

---
*MIT License | CodeAlpha Internship Project*

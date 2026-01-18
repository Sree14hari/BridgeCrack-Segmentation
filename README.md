# Bridge Crack Classification System

An automated Deep Learning pipeline to extract, measure, and classify bridge cracks from raw camera footage.

## 📌 Pipeline Overview
1.  **Patch Extraction:** Slices large raw images into $512 \times 512$ tiles.
2.  **Preprocessing:** Grayscale, Bilateral Filter (Denoise), and CLAHE (Contrast).
3.  **Auto-Sorting:** Measures crack width in pixels/mm and sorts into classes.
4.  **Augmentation:** Balances dataset via oversampling and offline augmentation.
5.  **Training:** Fine-tunes **MobileNetV2** (PyTorch) for classification.

## 🏷️ Classes (Engineering Standards)
* **Light:** $\le 0.1$ mm
* **Medium:** $0.1$ mm - $0.3$ mm
* **Heavy:** $> 0.3$ mm


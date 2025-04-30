
# ✨ Sign Language Recognition System (LSTM + MediaPipe)

A deep learning-based real-time gesture recognition system using computer vision and LSTM networks.

---

## 📁 Project Structure

```
MP_Data/                 # Preprocessed gesture data (npy files)
├── hi how are you/
├── thank you so much/
Logs/                    # TensorBoard logs
main.py                  # This code file
requirements.txt
README.md
```

---

## ⚙️ Requirements

Install dependencies using:

```bash
pip install -r requirements.txt
```

---

## 🚀 How to Run

1. **Prepare Data:**

   Ensure your directory follows this format:
   ```
   MP_Data/
   ├── hi how are you/
   │   ├── 0/
   │   │   ├── 0.npy
   │   │   ├── ...
   ├── thank you so much/
   ```

2. **Train the Model:**

   Run the script to train:

   ```bash
   python main.py
   ```

3. **Real-time Inference:**

   After training, the webcam feed will start. Perform gestures in front of your camera.

   Press `q` to quit.

---

## 🧠 Model Details

- **Architecture**: 3 LSTM layers + Dense layers
- **Input shape**: `(30, 1662)` — 30 frames, 1662 keypoints
- **Output**: Probability scores for each action

---

## 📊 Evaluation

After training:
- **Classification report** and **confusion matrix** are printed.
- Visualization shows real vs predicted gesture labels.

---

## 🖼️ Screenshots
- correct detection of the class "hello"
![image](https://github.com/user-attachments/assets/b38e7c61-1396-40ee-a2c0-9658716cbcc5)
- 📊Model Accuracy and loss during training
![WhatsApp Image 2025-03-29 at 17 51 24_c9d3a8d4](https://github.com/user-attachments/assets/26a8cd9e-9b4e-44aa-b4b7-275f1c4eb4a9)


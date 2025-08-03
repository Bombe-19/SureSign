## Signature Verification using Siamese Neural Network

This project uses a Siamese Neural Network to verify handwritten signatures and determine whether a signature is Genuine ✅ or Forged ❌. The model compares two input images and predicts similarity based on learned features.

---

## Model Used: Siamese Neural Network (SNN)

A **Siamese Neural Network** is a special type of neural network used to compare the similarity between two inputs. In this project, each "twin" of the SNN is a **Convolutional Neural Network (CNN)** that extracts features from the two input signature images. The model learns to distinguish genuine and forged signatures based on feature similarity.

---

## Why Siamese Neural Network?

- Works well with **few samples per class** (ideal for signature verification).
- Learns a **distance-based similarity function**, not just classification.
- Effective in **one-shot learning** tasks.
- Generalizes well to **new, unseen signatures** during inference.

---
## Accuracy
<img width="884" height="364" alt="image" src="https://github.com/user-attachments/assets/d4a25262-3b3c-4a12-89d4-4e314f10fc42" />


## CNN vs SNN

| Feature                | Convolutional Neural Network (CNN)       | Siamese Neural Network (SNN)                          |
|------------------------|------------------------------------------|--------------------------------------------------------|
| Input                 | Single image                              | Pair of images                                         |
| Output                | Class label                               | Similarity score (0 = Forged, 1 = Genuine)            |
| Task                  | Classification                           | Verification / Similarity Learning                    |
| Data Requirement      | Many samples per class                   | Fewer samples, just similar/dissimilar pairs          |
| Use Case              | Image classification, object detection   | Face/signature verification, one-shot learning        |

---

## Outcome

The model outputs a **similarity score** between two signature images. If the score is above a defined threshold (e.g., 0.5), the signatures are classified as **Genuine**, else **Forged**.

---


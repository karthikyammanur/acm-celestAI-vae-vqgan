# 🌠 CelestAI – Generative Models for Astronomical Image Synthesis

**ACM Research @ UT Dallas – Spring 2025**  
My contribution: Built and compared **VAE** and **VQGAN** deep learning models to generate synthetic astronomical images using the [Multimodal Universe Dataset](https://huggingface.co/datasets/MultimodalUniverse/legacysurvey).
---

## 🔭 Project Overview

To address data scarcity in astrophysical imaging, we explored how generative models like **Deep Convulutional GANs (DCGANs), StyleGANs, Variational Autoencoders (VAE), Vector Quantized GANs (VQGAN)** can synthesize high-fidelity images of galaxies and rare cosmic phenomena.

---

## 📁 Contents

- `models/vae.ipynb` – Implements a convolutional VAE for image reconstruction
- `models/vqgan.ipynb` – Implements a VQGAN with adversarial loss + vector quantization
- `assets/poster.png` – Final research poster for presentation

---

### 🧪 Results Summary

| Model     | Output Style        | Reconstruction Quality      | Notes                                                  |
|-----------|---------------------|------------------------------|--------------------------------------------------------|
| VAE       | Blurry, consistent  | ✓ Moderate loss, smooth maps | Reliable structure, lower detection metrics            |
| VQGAN     | Sharp, expressive   | ✓ Good visuals, fast runtime | Tradeoff between detail and model complexity           |
| StyleGAN  | Realistic, pretrained | ✓ Pretrained boost, high F1 | Benefited from large-scale transfer learning           |
| **DCGAN** | Clean, varied       | ✓ Best overall performance   | 🥇 Top recall/F1/ROC-AUC, best anomaly detection lift   |

> **DCGAN** achieved the **highest detection accuracy** (Recall 0.72, F1 Score 0.79, ROC-AUC 0.85) — improving recall by **15%** over baseline.  
> **VQGAN** showed a strong balance of performance and efficiency, making it suitable for scalable systems.


## 🖼️ Research Poster

<p align="center">
  <img src="assets/poster.png" alt="Poster" width="600"/>
</p>


<img width="1430" height="1069" alt="CelestAI_final_poster" src="https://github.com/user-attachments/assets/70b11c02-9edb-4c03-b32a-e6effd367950" />
[📄 Full Poster Download](assets/poster.png)

---

## 🚀 Run the Notebooks

You can open either model in **Google Colab**:

| Model | Notebook |
|-------|----------|
| VAE   | [Open in Colab](https://colab.research.google.com/github/karthikyammanur/celestai-research/blob/main/models/vae.ipynb) |
| VQGAN | [Open in Colab](https://colab.research.google.com/github/karthikyammanur/celestai-research/blob/main/models/vqgan.ipynb) |

---

## 🛠 Dependencies

pip install -r requirements.txt

## 👨‍💻 Team

Jagadeep Kalluri
Karthik Yammanur
Hrishikesh Naveenam
Shaheem Jaleel

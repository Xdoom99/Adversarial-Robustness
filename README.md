Adversarial Robustness on MNIST  Deep Learning + Cybersecurity

Explore, attack, defend, and detect adversarial examples on the MNIST dataset using deep learning. This notebook demonstrates how common neural networks can be broken using techniques like FGSM and PGD, and how to build defenses like adversarial training, detectors, and preprocessing pipelines.


- Understand adversarial attacks (FGSM, PGD) and their impact
- Train a robust CNN resistant to these attacks
- Build binary and multi-class adversarial detectors
- Use image processing defenses (like Gaussian blur)
- Visualize everything interactively and deploy as a demo


Core Components
Base CNN classifier trained on MNIST
FGSM (Fast Gradient Sign Method) attack
PGD (Projected Gradient Descent) attack
Adversarial training (defense-aware model)
Binary detector (Clean vs Adversarial)
Multi-class detector (Clean, FGSM, PGD)
Image defense using Gaussian blur
TensorBoard support for training logs
Interactive playground (ipywidgets)
Web UI with Gradio *(optional deployment)*

---

 Key Results

| Model                | Clean Acc | FGSM Acc | PGD Acc | Detector Acc |
|---------------------|-----------|----------|---------|---------------|
| Base CNN            | ~99%      | ~10%     | ~0%     | —             |
| After Adv Training  | ~97%      | ~90%     | ~65%    | —             |
| Binary Detector     | —         | —        | —       | >90%          |
| Multi-class Detector| —         | —        | —       | >85%          |
| Blur Defense (PGD)  | —         | —        | +10–20% | —             |

---

 Files

| File                            | Description                                        |
|---------------------------------|----------------------------------------------------|
| `Adversarial_Robustness_MNIST.ipynb` | Main notebook (Colab compatible)                |
| `README.md`                     | Project summary and usage                         |
| `requirements.txt`             | Python dependencies                               |
| `images/` *(optional)*         | Visualizations for README or documentation        |

---

 How to Run

1. Open `Adversarial_Robustness_MNIST.ipynb` in Google Colab  
2. Install required packages:

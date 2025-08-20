# Neural-Networks
This folder contains implementation of ML models using Neural Networks(Supervised, Unsupervised, Semi-supervised and Reinforcement Learning).

---

# 🌐 Neural Networks Across ML Paradigms

At the center, we have **Neural Networks (NNs)** — a flexible function approximator.
Depending on how we **train them** (data availability, loss function, feedback type), they can work in any ML setting.

---

## **1. Supervised Learning (Labeled Data)**

* **Definition**: Model learns mapping `X → Y` from labeled data.
* **NN Role**: Learns hidden representations that map input to target.
* **Common NN Architectures**:

  * **ANNs** – General prediction
  * **CNNs** – Images (classification, object detection)
  * **RNNs / Transformers** – Sequential data (text, speech, time series)
* **Examples**:
  ✅ Spam email classification
  ✅ Predicting house prices
  ✅ Medical diagnosis (tumor: benign vs malignant)

---

## **2. Unsupervised Learning (Unlabeled Data)**

* **Definition**: Model finds hidden structure without labels.
* **NN Role**: Learns compressed, latent representations.
* **Common NN Architectures**:

  * **Autoencoders (AE)** – Data compression, anomaly detection
  * **Variational Autoencoders (VAE)** – Generative modeling
  * **GANs** – Image & text generation
  * **Self-Organizing Maps (SOMs)** – Clustering
* **Examples**:
  ✅ Customer segmentation in marketing
  ✅ Image compression
  ✅ Generating new artworks (GANs)

---

## **3. Semi-Supervised Learning (Few Labels + Lots of Unlabeled Data)**

* **Definition**: Uses a mix of small labeled data & large unlabeled data.
* **NN Role**: Learns general representations from unlabeled data, then fine-tunes with labeled data.
* **Common NN Techniques**:

  * **Self-training with NNs** – Pseudo-labeling unlabeled samples
  * **SSL Transformers (like BERT, GPT pretraining)** – Train on unlabeled text, fine-tune for tasks
  * **Semi-Supervised GANs** – Generate & classify together
* **Examples**:
  ✅ Classifying medical images (few labeled MRI scans, many raw scans)
  ✅ Language tasks with little labeled data
  ✅ Fraud detection with few confirmed cases

---

## **4. Reinforcement Learning (Learning by Interaction)**

* **Definition**: Agent learns by trial-and-error, getting rewards/punishments.
* **NN Role**: Approximates **policy** (actions to take) or **value function** (expected reward).
* **Common NN Architectures**:

  * **Deep Q-Networks (DQN)** – Learn optimal actions
  * **Policy Gradient Methods** – Directly optimize decisions
  * **Actor-Critic Models** – Hybrid approach
* **Examples**:
  ✅ AlphaGo (beating humans at Go)
  ✅ Self-driving cars (steering, braking)
  ✅ Robotics & drones

---

# 🎨 Visual Flow (Aesthetic Layout)

```
                        ┌─────────────────────────┐
                        │   Neural Networks (NN)  │
                        │  (Flexible Learners)    │
                        └──────────┬──────────────┘
                                   │
         ┌─────────────────────────┼─────────────────────────┐
         │                         │                         │
         ▼                         ▼                         ▼
 ┌───────────────┐        ┌────────────────┐        ┌────────────────────┐
 │ Supervised    │        │ Unsupervised   │        │ Semi-Supervised    │
 │ Learning      │        │ Learning       │        │ Learning           │
 └───────────────┘        └────────────────┘        └────────────────────┘
         │                         │                         │
         ▼                         ▼                         ▼
   Classification,           Autoencoders,             SSL Transformers, 
   Regression, NLP           GANs, Clustering          Semi-GANs
         │                         │                         │
         └───────────────┬─────────┴─────────┬───────────────┘
                         ▼
                ┌──────────────────┐
                │ Reinforcement     │
                │ Learning          │
                └──────────────────┘
                         │
                         ▼
             Agents, Games, Robotics
```

---

# ✅ Final Takeaway

* **NNs are universal** → they can be used in **all ML paradigms**.
* The difference lies in:

  * The **type of data** (labeled, unlabeled, mixed, interactive).
  * The **loss function** & training approach.
  * The **architecture** (CNN, RNN, Transformer, GAN, etc.).

---


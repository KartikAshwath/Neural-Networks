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



---

# 🧠 Complete Concepts of Neural Networks (Roadmap + Teaching Guide)

---

## **1. Foundations**

Before NN, you need to recall:

* **Linear Algebra**: Vectors, matrices, dot product
* **Calculus**: Derivatives, chain rule (for backpropagation)
* **Probability & Stats**: Distributions, expectation, variance
* **ML Basics**: Supervised learning, loss functions, gradient descent

👉 Without these, NN will feel like “magic.”

---

## **2. Neurons & Perceptron**

* A **neuron** takes input → applies weights → adds bias → passes through activation function.
* Equation:

$$
z = w_1x_1 + w_2x_2 + \dots + w_nx_n + b
$$

$$
a = f(z)
$$

where:

* $w$ = weights
* $b$ = bias
* $f$ = activation function

👉 This is the “brain cell” of NN.

---

## **3. Architecture of a Neural Network**

* **Input layer** – features (e.g., pixels of an image)
* **Hidden layers** – multiple neurons stacked
* **Output layer** – prediction (class label, probability, regression value)

Example: Feedforward ANN

```
Input → Hidden Layer 1 → Hidden Layer 2 → Output
```

---

## **4. Activation Functions**

Why? Without them, NNs would just be linear regression.

* **Sigmoid**: S-shaped curve → (0,1) output
* **Tanh**: (-1,1) range → better than sigmoid sometimes
* **ReLU**: max(0, x) → most popular (avoids vanishing gradient)
* **Softmax**: for classification probabilities

---

## **5. Training a NN**

Training = Adjusting weights & bias to minimize **loss function**.

Steps:

1. **Forward Pass** → compute predictions.
2. **Loss Function** → measure error (MSE, Cross-Entropy).
3. **Backward Pass (Backpropagation)** → compute gradients via chain rule.
4. **Optimizer (Gradient Descent / Adam)** → update weights.

---

## **6. Important NN Concepts**

* **Bias-Variance Tradeoff** – underfitting vs overfitting
* **Regularization** – dropout, L1/L2 to avoid overfitting
* **Batch Normalization** – stabilizes training
* **Learning Rate** – how fast weights update
* **Epochs, Batches** – control training cycles

---

## **7. Types of Neural Networks**

* **Feedforward (ANN/MLP)** – basics, tabular data
* **Convolutional NN (CNN)** – images, spatial data
* **Recurrent NN (RNN, LSTM, GRU)** – sequential data (time series, NLP)
* **Transformers** – modern NLP/vision (ChatGPT, BERT, etc.)
* **GANs (Generative Adversarial Networks)** – image synthesis, generation
* **Autoencoders** – compression, anomaly detection

---

## **8. Applications**

* Computer Vision (face recognition, object detection)
* NLP (chatbots, translation, summarization)
* Speech (voice assistants, transcription)
* Healthcare (disease detection)
* Finance (fraud detection, stock prediction)

---

## **9. Practical Workflow**

1. Collect + preprocess data
2. Split into train/val/test
3. Choose NN architecture
4. Train (forward + backprop)
5. Evaluate performance
6. Tune hyperparameters

---

## **10. Limitations of Neural Networks**

* Data-hungry (need lots of data)
* Computationally expensive (need GPUs/TPUs)
* Black-box (hard to interpret)
* Overfitting risk

---

✅ That’s the **roadmap overview**.
We can now go **step by step in detail**:

* First: **Neuron + Perceptron**
* Then: **Activation Functions**
* Then: **Backpropagation**
* And so on…

---

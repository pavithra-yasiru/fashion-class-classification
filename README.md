# 👗 Fashion MNIST Classification using CNN

A deep learning project to classify images of fashion items into 10 categories using the **Fashion MNIST dataset** and a **Convolutional Neural Network (CNN)**.

---

## 🧾 Problem Statement

The dataset contains **70,000 grayscale images** (60,000 train / 10,000 test) sized **28×28 pixels**. Each image represents a clothing item from 10 classes:

| Label | Class       |
|-------|-------------|
| 0     | T-shirt/top |
| 1     | Trouser     |
| 2     | Pullover    |
| 3     | Dress       |
| 4     | Coat        |
| 5     | Sandal      |
| 6     | Shirt       |
| 7     | Sneaker     |
| 8     | Bag         |
| 9     | Ankle boot  |

---

## 🎯 Business Case

Accurate fashion image classification benefits:
- **E-commerce**: Automated product tagging and search filters.
- **Retail analytics**: Inventory categorization and forecasting.
- **Recommendation systems**: Suggesting similar or complementary items.

---

## 📊 Dataset

- **Source**: [Fashion MNIST by Zalando](https://github.com/zalandoresearch/fashion-mnist)  
- **Format**: 28×28 grayscale images  
- **Classes**: 10 (clothing types)  
- **Size**: 70,000 images (60,000 train, 10,000 test)

---

## ⚙️ Data Preprocessing

1. Normalized pixel values to **0-1 range**.  
2. Reshaped images to **(28, 28, 1)** for CNN input.  
3. Converted labels to **integer categories**.

---

## 🏗️ Model Architecture

Implemented a **Convolutional Neural Network (CNN)**:

1. **Conv2D Layer** – 64 filters, 3×3 kernel, ReLU activation  
2. **Dense Layer** – 64 units, ReLU activation  
3. **Output Layer** – 10 units, Sigmoid activation (multi-class)

**Compilation**:  
- Optimizer: Adam (lr=0.001)  
- Loss: Sparse Categorical Crossentropy  
- Metric: Accuracy

---

## 🚀 Training & Evaluation

- Trained on 60,000 samples, tested on 10,000 samples.
- Evaluated using:
  - **Test Accuracy**
  - **Confusion Matrix**
  - **Training/Validation Accuracy & Loss curves**

---

## 📈 Results

- **Test Accuracy**: *(Add your accuracy, e.g., 88%)*
- **Confusion Matrix**:  
*(Insert confusion matrix plot here)*
- **Accuracy & Loss Plots**:  
*(Insert accuracy/loss plots here)*

---

## 📂 Project Structure

```
Fashion-MNIST-Classification/
│── Fashion MNIST.ipynb             # Jupyter notebook with code
│── README.md                       # Project documentation
│── requirements.txt                # Dependencies
│── fashion-mnist_train_part{i}.csv # Training data sets (need to append)
│── fashion-mnist_test.csv          # Test data set
```

---

## 🔧 Installation & Usage

### 1. Clone repository
```bash
git clone https://github.com/your-username/Fashion-MNIST-Classification.git
cd Fashion-MNIST-Classification
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run notebook
```bash
jupyter notebook "Fashion MNIST.ipynb"
```

---

## 🛠 Future Improvements

- Add **data augmentation** (rotation, flipping) for better generalization.
- Experiment with **deeper CNN architectures** (e.g., ResNet).
- Deploy as a **web app** using Streamlit or Flask.

---

## 🏷 License

This project is licensed under the MIT License.

# VU-DL-Lab-Setup

## 🚀 **Setup Guide**

This project supports **both TensorFlow and PyTorch**.  
⚠️ **Do not install both frameworks in the same virtual environment.** Create **separate environments** and select the appropriate one in Jupyter.

### 1️⃣ Install Git
```bash
sudo apt update
sudo apt install git
```

### 2️⃣ Clone the Repository
```bash
git clone [https://github.com/vaidhav-adit/VU-DL-Lab-Setup.git](https://github.com/vaidhav-adit/VU-DL-Lab-Setup.git)
cd VU-DL-Lab
cd Setup
```

**If the above steps did not work you can manually clone the repo by just downloading it as a ZIP file.**

---

## 🧪 Environment Setup

Choose one of the following options based on the framework you want to use.

### 🔶 Option A: TensorFlow Environment

**Create a virtual environment:**
```bash
python3 -m venv tensorflow_env
```

**Activate the environment:**
```bash
source tensorflow_env/bin/activate
```

**Install dependencies:**
```bash
pip install --upgrade pip
pip install -r tensorflow_requirements.txt
```

**Add the environment as a Jupyter kernel:**
```bash
python -m ipykernel install --user --name=tensorflow_env --display-name "Python (tensorflow_env)"
```

### 🔷 Option B: PyTorch Environment

**Create a virtual environment:**
```bash
python3 -m venv pytorch_env
```

**Activate the environment:**
```bash
source pytorch_env/bin/activate
```

**Install dependencies:**
```bash
pip install --upgrade pip
pip install -r pytorch_requirements.txt
```

**Add the environment as a Jupyter kernel:**
```bash
python -m ipykernel install --user --name=pytorch_env --display-name "Python (pytorch_env)"
```

---

## 📓 Using Jupyter Notebook

**Launch Jupyter Notebook:**

1. `jupyter notebook`
2. Open a notebook
3. Go to **Kernel**
4. Select the appropriate kernel we just created: `Python (tensorflow_env)` for TensorFlow OR `Python (pytorch_env)` for PyTorch

**After completion you are good to go!**

# Lab 1:
In this lab the following concepts are covered -> 
1. **Tensor Fundamentals:** Establishes the core multi-dimensional data structure of Deep Learning, detailing key attributes such as rank, shape, and float precision.
2. **Critical Operations:** Covers essential tensor manipulations—including reshaping, flattening, and dimension broadcasting—to effectively structure data for neural network layers.
3. **Data Pipelines:** Demonstrates the construction of robust pipelines utilizing DataLoader for efficient batching, shuffling, and normalization of the MNIST dataset.
4. **Framework Agnostic:** Emphasizes universal principles of tensor manipulation and preprocessing that are implemented in PyTorch but are equally essential for TensorFlow workflows.

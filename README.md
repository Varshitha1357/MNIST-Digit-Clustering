# 🧠 Digit Clustering with t-SNE & K-Means (Unsupervised Learning)

An interactive **unsupervised machine learning project** that explores clustering patterns in handwritten digit images using **t-SNE dimensionality reduction** and **K-Means clustering**.

The application is built with **Streamlit** and allows users to interactively visualize how structure emerges in image data **without using labels during training**.

---

## 🚀 Project Highlights

- 🔍 Unsupervised clustering of handwritten digits
- 📉 Dimensionality reduction using **t-SNE**
- 📊 Interactive 2D visualization with **Plotly**
- 🎛️ Real-time control over clustering & t-SNE parameters
- 📈 Evaluation using **Silhouette Score** and **post-hoc accuracy**
- 🌐 Interactive **Streamlit web application**

---

## 🖼️ Screenshots

*(All screenshots are stored in the `docs/` folder)*

![Clustering Visualization](docs/image1.png)
![t-SNE Projection](docs/image2.png)
![Cluster Distribution](docs/image3.png)
![Evaluation Metrics](docs/image4.png)

---

## 🧩 Why t-SNE + K-Means?

- Image data is **high-dimensional**, making direct clustering ineffective
- **t-SNE** preserves local neighborhood structure when projecting data into 2D
- **K-Means** clusters visually similar digits in the reduced space
- This combination improves **interpretability and visualization**, not supervised accuracy

> ⚠️ t-SNE is used only for **exploration and visualization**, not as a production embedding method.

---

## 📊 Dataset

This project uses the **Digits dataset** from `scikit-learn`:

- **1,797 samples**
- **8 × 8 grayscale images**
- **64 numerical features**
- **10 digit classes (0–9)**

> Note: This is **not the original MNIST dataset (28×28)**.  
> It is the smaller Digits dataset provided by `sklearn.datasets.load_digits`.

---

## 📐 Metrics Explained

### 🔹 Silhouette Score
Measures how well data points fit within their assigned cluster.

- Range: **–1 to 1**
- Higher values indicate better cluster separation

### 🔹 Post-hoc Accuracy
Clusters are mapped to digit labels **after clustering** using majority voting.

> This metric is for **evaluation only** and should not be interpreted as supervised accuracy.

---

## 🎛️ Application Controls

- **Number of clusters (k)**: 3–15
- **t-SNE Perplexity**: 5–50 (controls local vs global structure)
- **Random State**: Ensures reproducibility

Changes are reflected **in real time**.

---

## 🛠️ Tech Stack

- **Python 3.11**
- **Streamlit** – interactive web app
- **scikit-learn** – machine learning
- **Plotly** – interactive charts
- **NumPy** – numerical computation
- **Pillow** – image processing

---

## 📁 Project Structure

```
MNIST-Clustering-Project/
│
├── app.py                 # Main Streamlit application
├── requirements.txt       # Python dependencies
├── pyproject.toml         # Poetry configuration (optional)
├── README.md              # Project documentation
├── .gitignore             # Ignored files & folders
└── docs/                  # Screenshots used in README
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/Varshitha1357/MNIST-Digit-Clustering.git
cd MNIST-Digit-Clustering
```

### 2️⃣ Create a Virtual Environment (Recommended)
```bash
python -m venv venv
source venv/bin/activate   # Linux / macOS
venv\Scripts\activate      # Windows
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Run the Application
```bash
streamlit run app.py
```

Open in browser:
```
http://localhost:8501
```

---

## 📦 requirements.txt
All required libraries are listed to ensure reproducibility.

---

## 🚫 .gitignore (Included)
```
# Virtual environments
venv/
.env/

# Python cache
__pycache__/
*.pyc

# Streamlit
.streamlit/

# OS files
.DS_Store
Thumbs.db
```

---

## 🌱 Learning Outcomes

- Understanding unsupervised learning on image data
- Strengths and limitations of K-Means
- Visualizing high-dimensional data
- Correct evaluation of clustering models
- Building interactive ML applications with Streamlit

---

## 🔮 Future Improvements

- PCA vs t-SNE vs UMAP comparison
- Automatic optimal-k selection
- Confusion matrix after cluster-label mapping
- Support for real MNIST (28×28) dataset
- Performance optimization with caching

---

## 👤 Author

**Varshitha Yejerla**  
Aspiring AI/ML Engineer  
Focused on building conceptually strong and production-ready ML projects

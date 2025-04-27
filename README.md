# script-mix-GARAJ  
**Mixing Scripts for Low-resource Language Parsing**  

## Overview  
Script Mix is executed with the following pipeline:  

1. **Data loading and preprocessing.**  
2. **MBERT model** with pre-trained knowledge of major languages worldwide.  
3. **Training language adapters** with both original and transliterated scripts of a new low-resource language separately.  
4. **Fusing these two Language Adapters** using Adapter Fusion Plus.  
5. **Training a new task adapter** upon this for POS Tagging and Dependency Parsing.  

The code is available in **`script-mix-GARAJ.ipynb`**.  

---

## How to Run the Code Locally?  

### Prerequisites  

Ensure you have the following installed:  
- **Python (≥3.x)**  
- **Jupyter Notebook**  
- **PyTorch with CUDA support**

### 1. Clone the Repository  

- **git clone https://github.com/your-username/script-mix-GARAJ.git**
- **cd script-mix-GARAJ**

### 2. Create a CONDA environment

- **conda create --name scriptmix python=3.x**
- **conda activate scriptmix**

### 3. Install Dependencies

- **git clone https://github.com/adapter-hub/adapters.git**
- **pip install -r requirements.txt**

### 4. Launch Jupyter Notebook

- **jupyter notebook**

Then open distilbert-and-unipelt.ipynb and execute the cells sequentially.

## How to Run the Code over Google Colab?  

1. **Load the .ipynb file onto Google Colab.**
2. **Upload the .conllu dataset files of the language (train, dev, test) to the colab file.**
3. **Run all the cells at your own pace.**

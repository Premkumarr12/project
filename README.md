<!--
Copyright (c) 2025 Your Name.

Released under the MIT License.
See https://opensource.org/licenses/MIT
-->



<p align="center">
  <a href="https://github.com/sangsaist/sih-edna-classifier/stargazers">
    <img alt="GitHub stars" src="https://img.shields.io/github/stars/sangsaist/sih-edna-classifier?style=social">
  </a>
  <a href="https://github.com/sangsaist/sih-edna-classifier/network/members">
    <img alt="GitHub forks" src="https://img.shields.io/github/forks/sangsaist/sih-edna-classifier?style=social">
  </a>
  <a href="https://github.com/sangsaist/sih-edna-classifier/actions">
    <img alt="Build Status" src="https://img.shields.io/github/actions/workflow/status/sangsaist/sih-edna-classifier/ci.yml?branch=main">
  </a>
  <a href="https://opensource.org/licenses/MIT">
    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-blue.svg">
  </a>
  <a href="#">
    <img alt="Python" src="https://img.shields.io/badge/python-3.9%2B-blue">
  </a>
</p>

<h1 align="center">🧬 eDNA Biodiversity — Taxonomy & Biodiversity from DNA Sequences</h1>

<p align="center">
  <em>AI-powered taxonomy identification and biodiversity assessment from raw environmental DNA (eDNA) datasets using DNABERT and clustering.</em>
</p>

---
## 📖 Project Overview  
This project leverages **AI-powered DNA sequence analysis** to identify taxonomy and assess biodiversity from raw environmental DNA (eDNA) datasets.  

### 🔁 Workflow  
**Input (User):** Raw eDNA data provided by researchers or labs.  
**Process:**  
- Learns sequence patterns (DNABERT embeddings)  
- Matches with known species (**Supervised Classification**)  
- Groups novel sequences into clusters (**Unsupervised Clustering**)  
- Stores clusters for future reference & comparison    

**Output (Dashboard):**  
- Species list & taxonomy  
- Abundance & diversity indices  
- Novelty alerts for potentially unknown or rare species  

---

## 🌟 Features  
-  **High computational cost optimization** → Uses **pre-trained DNABERT models** with light fine-tuning.  
-  **Limited eDNA datasets in India** → Prototype dataset for India + integration with public repositories.
-  **Validation of novel species** → Confidence scoring + expert/BLAST verification.  
-  **Integration with standards** → Compatible with existing bioinformatics pipelines.  

---

## 🧰 Tech Stack  
- **Programming:** Python  
- **Frameworks:** PyTorch, HuggingFace Transformers  
- **Core Model:** DNABERT (fine-tuned for marine eDNA)  
- **Visualization:** Streamlit + Plotly (interactive charts & dashboard)  
- **Data Sources:** NCBI, BLAST, SILVA, BOLD, Marine eDNA samples  

---

## 🖥️ Installation & Setup  

### 📦 Requirements  
- Flask>=2.0
- streamlit>=1.27
- pandas>=1.5
- numpy>=1.23
- plotly>=5.17
- torch>=2.0
- transformers>=4.30
- umap-learn>=0.5
- hdbscan>=0.8
- scikit-learn>=1.2

### ▶️ Run the Application  
```bash
# Clone the repository
git clone https://github.com/your-username/edna-biodiversity.git
cd edna-biodiversity

# Install dependencies
pip install -r requirements.txt

# Run the app
streamlit run app.py
```

### 📂 Sample Dataset
```bash
Example input record:

18S_00287,TCCGTTTGTCCTGAGAGTAAC...,18S,ColdWater_Coral_A,CCLME,AbyssalPlain_B,147.0,species,0.91,AbyssalPlain_B,3885.0

```
### 🔮 Future Improvements

        🌐 Expand datasets with more India-specific eDNA samples.

        🧠 Improve unsupervised clustering techniques.

        🧬 Collaborate with marine biologists for expert validation.

        📈 Add real-time biodiversity trend analysis.

## 📜 License
Released under the [MIT License](./LICENSE).


## 🙌 Acknowledgments
- [NCBI](https://www.ncbi.nlm.nih.gov/)
- [SILVA Database](https://www.arb-silva.de/)
- [BOLD Systems](https://www.boldsystems.org/)
- [Hugging Face Transformers](https://huggingface.co/transformers)

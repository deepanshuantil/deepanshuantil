# Hi, I'm Deepanshu 👋

**Junior Data Engineer** · MSc Computer Science (Distinction), University of Hertfordshire · Based in Slough / London, UK

I build data pipelines that are **traceable, tested and reproducible**: raw files in, clean and checked data out, with every decision written down. I also have a background in deep learning for medical imaging.

🔭 Currently: finishing an end-to-end **NHS GP appointments pipeline** (PySpark → DuckDB → Streamlit) as part of a data engineering internship
🎯 Open to: **Data Engineering roles in London** (on-site, hybrid or remote)
💬 Connect: [LinkedIn](https://www.linkedin.com/in/deepanshu-antil)

---

## 🛠️ Tech stack

| Area | Tools |
|---|---|
| **Languages** | Python, SQL |
| **Data engineering** | PySpark / Apache Spark, pandas, DuckDB, Parquet, ETL pipelines, star schema modelling |
| **Data quality & testing** | pytest, automated reconciliation checks, data profiling |
| **Visualisation** | Streamlit, Plotly, Matplotlib, Seaborn |
| **Machine learning** | TensorFlow / Keras, PyTorch, timm, scikit-learn, Albumentations |
| **Tools** | Git, GitHub, Jupyter, Kaggle, Google Colab |

---

## 📌 Featured projects

### 🏥 [NHS GP Appointments ETL Pipeline](https://github.com/deepanshuantil/lsa-oct-2026)
End-to-end pipeline on real NHS England GP appointment data (~1.55M rows across three files).
- **Extract:** copies raw files, fixes a mislabelled Excel file, and records size, SHA-256 and row count for every file in a manifest
- **Transform (PySpark):** explicit schemas; fixes five data traps (fake CSV, hidden BOM, day-first dates, duplicate-looking rows that are real appointments, inconsistent labels) while keeping the total at exactly **742,804,525 appointments**
- **Load (DuckDB):** star schema with 3 fact tables and 5 dimensions; reloading changes nothing
- **Quality:** **46 pytest tests** and **9/9 automated quality checks** passing; 159 MB of CSV reduced to **5.6 MB of Parquet**
- Every design choice recorded in a decision log

`Python` `PySpark` `DuckDB` `Parquet` `pytest` `ETL` `Data Modelling`

### 🩻 [Chest X-ray Pneumonia Classification](https://github.com/deepanshuantil/chest-xray-pneumonia-classification)
Deep learning model that classifies paediatric chest X-rays as Normal, Bacterial Pneumonia or Viral Pneumonia.
- Turned a 2-class dataset (5,856 X-rays) into a 3-class problem and balanced it with augmentation
- Compared four transfer-learning models: **ViT-B/16 87.7%**, EfficientNet-B5 87.1%, Xception 87.1%, ResNet-50 85.1% test accuracy
- Error analysis showed most mistakes were bacterial vs viral confusion; F1 0.97 on Normal cases

`Python` `PyTorch` `TensorFlow` `Computer Vision` `Transfer Learning`

---

<sub>Feel free to explore the repos or reach out on LinkedIn.</sub>

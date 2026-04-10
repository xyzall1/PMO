# PMO: Pipeline Optimization dengan Machine Learning

Repository ini berisi implementasi dan optimasi pipeline machine learning menggunakan beberapa teknik advanced, termasuk TPOT (Tree-based Pipeline Optimization Tool), PSO (Particle Swarm Optimization), dan Histogram Gradient Boosting.

## 📋 Daftar Isi

- [Tentang Project](#tentang-project)
- [Struktur Repository](#struktur-repository)
- [Teknologi yang Digunakan](#teknologi-yang-digunakan)
- [File-file Utama](#file-file-utama)
- [Instalasi & Setup](#instalasi--setup)
- [Penggunaan](#penggunaan)
- [Hasil & Performa](#hasil--performa)
- [Kontribusi](#kontribusi)
- [Lisensi](#lisensi)

## 🎯 Tentang Project

PMO (Pipeline Optimization) adalah project yang fokus pada:

- **Optimasi Hyperparameter**: Menggunakan PSO dan TPOT untuk menemukan hyperparameter terbaik
- **Pipeline Building**: Membangun dan mengoptasi pipeline machine learning secara otomatis
- **Model Comparison**: Membandingkan performa berbagai model machine learning
- **Advanced Boosting**: Implementasi Histogram Gradient Boosting untuk performa optimal

## 📁 Struktur Repository

```
PMO/
├── HistGradientBoosting_Model.ipynb    # Model HGB standalone
├── TPOT_&_PSO_HGB.ipynb               # Kombinasi TPOT, PSO, dan HGB
└── README.md                           # Dokumentasi project
```

## 🛠️ Teknologi yang Digunakan

### Machine Learning & Optimization
- **Scikit-learn**: Library utama untuk machine learning
- **TPOT**: Automated machine learning pipeline optimization
- **PSO (Particle Swarm Optimization)**: Metaheuristic optimization algorithm
- **XGBoost / HistGradientBoosting**: Advanced gradient boosting algorithms

### Data Processing
- **Pandas**: Data manipulation dan analysis
- **NumPy**: Numerical computing

### Visualization & Analysis
- **Matplotlib**: Data visualization
- **Seaborn**: Statistical data visualization

## 📚 File-file Utama

### 1. HistGradientBoosting_Model.ipynb
**Deskripsi**: Implementasi standalone model Histogram Gradient Boosting

**Konten Utama**:
- Loading dan preprocessing data
- Training Histogram Gradient Boosting model
- Hyperparameter tuning
- Model evaluation (accuracy, precision, recall, F1-score)
- Visualization hasil prediksi dan feature importance

**Output**: Model HGB yang teroptasi dengan performa metrik lengkap

---

### 2. TPOT_&_PSO_HGB.ipynb
**Deskripsi**: Kombinasi TPOT dan PSO untuk optimasi pipeline machine learning dengan HGB

**Konten Utama**:
- Automated pipeline optimization menggunakan TPOT
- Particle Swarm Optimization untuk fine-tuning hyperparameter
- Comparison antara berbagai konfigurasi pipeline
- Cross-validation dan evaluation metrics
- Visualization perbandingan model performa

**Output**: Optimized pipeline dengan hasil perbandingan comprehensive

---

## 🚀 Instalasi & Setup

### Prerequisites
- Python 3.7+
- Jupyter Notebook atau JupyterLab
- pip atau conda package manager

### Installation Steps

1. **Clone Repository**
```bash
git clone https://github.com/xyzall1/PMO.git
cd PMO
```

2. **Install Dependencies**
```bash
pip install -r requirements.txt
```

Jika file `requirements.txt` belum ada, install packages berikut:
```bash
pip install pandas numpy scikit-learn xgboost tpot matplotlib seaborn jupyter
```

3. **Buka Jupyter Notebook**
```bash
jupyter notebook
```

Atau untuk JupyterLab:
```bash
jupyter lab
```

## 📖 Penggunaan

### Menjalankan HistGradientBoosting_Model.ipynb
1. Buka file `HistGradientBoosting_Model.ipynb` di Jupyter
2. Pastikan dataset sudah tersedia di path yang sesuai
3. Run semua cell secara berurutan (Shift + Enter)
4. Analisis hasil metrics dan visualization

**Output yang Diharapkan**:
- Trained model object
- Performance metrics (accuracy, precision, recall, F1-score)
- ROC-AUC curve
- Feature importance plot
- Confusion matrix

### Menjalankan TPOT_&_PSO_HGB.ipynb
1. Buka file `TPOT_&_PSO_HGB.ipynb` di Jupyter
2. Jalankan cell untuk TPOT optimization (dapat memakan waktu beberapa menit)
3. Jalankan PSO optimization untuk fine-tuning
4. Bandingkan hasil kedua method

**Output yang Diharapkan**:
- Generated pipeline code dari TPOT
- Optimized hyperparameters dari PSO
- Comparison table antara berbagai konfigurasi
- Best performing model configuration

### Tips untuk Performa Optimal
- **Memory**: Jalankan di environment dengan RAM minimal 4GB
- **Time**: TPOT optimization bisa memakan 10-30 menit tergantung dataset size
- **Dataset**: Pastikan data sudah di-split menjadi train dan test set
- **Hyperparameter**: Adjust iteration dan population size di PSO sesuai kebutuhan

## 📊 Hasil & Performa

### Expected Performance Metrics

| Metrik | Deskripsi |
|--------|-----------|
| **Accuracy** | Proporsi prediksi yang benar |
| **Precision** | Akurasi positif prediction |
| **Recall** | Coverage true positive |
| **F1-Score** | Harmonic mean precision & recall |
| **ROC-AUC** | Area under ROC curve |

### Optimization Results

- **TPOT**: Menghasilkan pipeline otomatis dengan performa terbaik
- **PSO**: Fine-tuning hyperparameter dengan convergence yang baik
- **HGB**: Excellent performance untuk classification tasks

## 💡 Key Features

✅ **Automated Pipeline Building** - TPOT mengotomatisasi pipeline construction
✅ **Metaheuristic Optimization** - PSO untuk hyperparameter tuning
✅ **Advanced Boosting** - Histogram Gradient Boosting implementation
✅ **Comprehensive Evaluation** - Multiple metrics dan cross-validation
✅ **Visualization** - Plot dan chart untuk interpretasi hasil
✅ **Reproducible** - Seed management untuk hasil yang konsisten

## 📝 Catatan Penting

1. **Dataset**: Pastikan dataset sudah pre-processed (missing values handling, feature scaling)
2. **Runtime**: Optimization process bisa memakan waktu signifikan (10-60 menit)
3. **Memory Usage**: Monitor memory usage saat running TPOT dengan dataset besar
4. **Random Seed**: Set random seed untuk reproducibility
5. **Hardware**: Recommended menggunakan GPU untuk performa lebih cepat

## 🔄 Workflow Typical

```
Data Loading
    ↓
Data Preprocessing & Exploration
    ↓
Feature Engineering (optional)
    ↓
Train-Test Split
    ↓
TPOT Pipeline Optimization
    ↓
PSO Hyperparameter Tuning
    ↓
Model Evaluation
    ↓
Result Comparison & Visualization
    ↓
Export Model & Results
```

## 🤝 Kontribusi

Kontribusi sangat welcome! Silakan:

1. Fork repository ini
2. Buat branch baru (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push ke branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request

## 📝 Lisensi

Project ini tersedia di bawah lisensi MIT. Lihat file LICENSE untuk detail lebih lanjut.

## 👤 Author

**xyzall1** - [GitHub Profile](https://github.com/xyzall1)

---

## 📚 Referensi & Bacaan Lanjutan

- [TPOT Documentation](http://epistasislab.github.io/tpot/)
- [Scikit-learn User Guide](https://scikit-learn.org/stable/user_guide.html)
- [XGBoost Documentation](https://xgboost.readthedocs.io/)
- [PSO Algorithm](https://en.wikipedia.org/wiki/Particle_swarm_optimization)
- [Histogram Gradient Boosting](https://scikit-learn.org/stable/modules/ensemble.html#histogram-based-gradient-boosting)

---

## ❓ FAQ

**Q: Berapa lama waktu yang dibutuhkan untuk menjalankan TPOT?**
A: Tergantung dataset size dan resources. Biasanya 10-30 menit untuk dataset medium.

**Q: Apakah bisa running di Google Colab?**
A: Ya! Google Colab memiliki resources yang cukup dan sudah pre-installed scikit-learn.

**Q: Gimana cara adjust jumlah iteration di PSO?**
A: Cari parameter `n_iterations` atau `iterations` di cell PSO, kemudian ubah nilainya.

**Q: Model mana yang paling baik?**
A: Tergantung dataset dan use case. Biasanya HGB atau hasil TPOT memberikan performa terbaik.

---

## 📞 Support

Jika ada pertanyaan atau issue, silakan buka GitHub Issue di repository ini.

---

**Last Updated**: 2026
**Status**: Active Development

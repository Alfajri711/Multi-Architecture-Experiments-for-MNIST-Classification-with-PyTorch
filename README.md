# Eksperimen Multi-Arsitektur untuk Klasifikasi MNIST dengan PyTorch

Selamat datang di repository **Eksperimen Multi-Arsitektur untuk Klasifikasi MNIST dengan PyTorch**! Proyek ini bertujuan untuk mengeksplorasi performa klasifikasi dataset MNIST menggunakan berbagai arsitektur jaringan saraf. Dengan PyTorch sebagai framework utama, proyek ini memfasilitasi eksperimen komprehensif untuk memahami bagaimana kedalaman model, fungsi aktivasi, dan fungsi loss memengaruhi hasil klasifikasi.

---

## 🌟 **Tentang Proyek**  
Dataset **MNIST** merupakan kumpulan gambar angka tangan tertulis (0-9) yang sering digunakan sebagai benchmark dalam machine learning. Dalam proyek ini, kami mengimplementasikan tiga arsitektur jaringan saraf yang berbeda untuk membandingkan performa mereka dalam mengklasifikasi dataset MNIST.  

---

## ⚙️ **Fitur Utama**  

1. **🧠 Tiga Arsitektur Model Jaringan Saraf**:
   - **ShallowModel**: Model sederhana dengan 1 lapisan tersembunyi berisi 64 unit.
   - **MediumModel**: Model menengah dengan 2 lapisan tersembunyi masing-masing 128 dan 64 unit.
   - **DeepModel**: Model kompleks dengan 3 lapisan tersembunyi masing-masing 256, 128, dan 64 unit.

2. **⚡ Fungsi Aktivasi**:
   - Mendukung eksperimen dengan tiga fungsi aktivasi: **ReLU**, **Sigmoid**, dan **Tanh**.

3. **📉 Eksperimen Fungsi Loss**:
   - **Cross Entropy Loss**
   - **Sparse Cross Entropy Loss**
   - **Hinge Loss**  
   Eksperimen ini membantu memahami bagaimana fungsi loss memengaruhi pembelajaran model.

4. **📊 Evaluasi Komprehensif**:
   Model yang sudah dilatih dievaluasi menggunakan:
   - **Akurasi**
   - **Presisi**
   - **Recall**
   - **F1-Score**
   - **Confusion Matrix**  
   Evaluasi ini memberikan wawasan lengkap mengenai performa model.

5. **🚀 Pelatihan Fleksibel**:
   - Optimizer **Adam** dengan learning rate 0,001.
   - Pelatihan dilakukan selama 10 epoch untuk setiap konfigurasi.

---

## 🔍 **Hasil Evaluasi**  

### Performa Model Berdasarkan Arsitektur  
| Model           | Fungsi Aktivasi | Fungsi Loss         | Akurasi | Presisi | Recall | F1-Score |
|------------------|----------------|---------------------|---------|---------|--------|----------|
| ShallowModel     | ReLU           | CrossEntropyLoss    | 96.2%   | 96.1%   | 95.8%  | 95.9%    |
| MediumModel      | Tanh           | SparseCrossEntropy  | 97.4%   | 97.3%   | 97.1%  | 97.2%    |
| DeepModel        | Sigmoid        | HingeLoss           | 98.5%   | 98.4%   | 98.3%  | 98.3%    |

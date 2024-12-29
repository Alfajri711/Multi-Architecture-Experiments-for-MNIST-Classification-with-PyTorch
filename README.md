# 🎉 **Eksperimen Multi-Arsitektur untuk Klasifikasi MNIST dengan PyTorch** 🎉

Selamat datang di proyek **Eksperimen Multi-Arsitektur untuk Klasifikasi MNIST**! Di sini, kami akan mengeksplorasi dan membandingkan kinerja berbagai arsitektur jaringan saraf dalam mengklasifikasikan dataset MNIST menggunakan **PyTorch**. Kami menguji berbagai kombinasi **fungsi aktivasi** dan **fungsi loss** untuk melihat bagaimana kedalaman model, tipe aktivasi, dan fungsi loss memengaruhi hasil klasifikasi.

## 📚 **Deskripsi Proyek**

### **🧠 Model Jaringan Saraf:**
Kami menguji tiga model dengan jumlah lapisan tersembunyi yang berbeda untuk melihat bagaimana kedalaman model mempengaruhi performa:
- **ShallowModel**: 1 lapisan tersembunyi dengan 64 unit.
- **MediumModel**: 2 lapisan tersembunyi dengan 128 dan 64 unit.
- **DeepModel**: 3 lapisan tersembunyi dengan 256, 128, dan 64 unit.

### **💡 Fungsi Aktivasi:**
Kami mengeksplorasi tiga fungsi aktivasi yang umum digunakan:
- **ReLU**: Membantu mempercepat pelatihan dan meningkatkan konvergensi.
- **Sigmoid**: Fungsi aktivasi untuk klasifikasi dengan output probabilitas.
- **Tanh**: Memungkinkan model untuk mempelajari representasi lebih kaya dengan output dalam rentang (-1, 1).

### **⚖️ Fungsi Loss:**
Fungsi loss mengukur seberapa baik model kita dalam mengklasifikasikan data:
- **Cross-Entropy Loss**: Digunakan untuk klasifikasi probabilistik.
- **Sparse Cross-Entropy Loss**: Untuk data dengan label integer.
- **Hinge Loss**: Sering dipakai pada model SVM untuk margin antar kelas.

### **📊 Evaluasi Model:**
Kami mengevaluasi performa model dengan berbagai metrik untuk mendapatkan gambaran menyeluruh tentang kemampuannya:
- **Akurasi**: Persentase prediksi yang benar.
- **Presisi, Recall, dan F1-Score**: Untuk memahami keseimbangan hasil positif dan negatif.
- **Confusion Matrix**: Memberikan gambaran visual tentang kesalahan klasifikasi model.

## 🏆 **Hasil Eksperimen** 🏆

### **💡 ReLU Activation - Cross-Entropy Loss:**
- **Shallow Model**: Akurasi = 97.11%
- **Medium Model**: Akurasi = 98.28%
- **Deep Model**: Akurasi = 98.43%

### **💡 ReLU Activation - Sparse Cross-Entropy Loss:**
- **Shallow Model**: Akurasi = 97.32%
- **Medium Model**: Akurasi = 98.15%
- **Deep Model**: Akurasi = 98.43%

### **💡 ReLU Activation - Hinge Loss:**
- **Shallow Model**: Akurasi = 96.83%
- **Medium Model**: Akurasi = 97.72%
- **Deep Model**: Akurasi = 98.02%

### **💡 Sigmoid Activation - Cross-Entropy Loss:**
- **Shallow Model**: Akurasi = 97.30%
- **Medium Model**: Akurasi = 98.30%
- **Deep Model**: Akurasi = 98.29%

### **💡 Sigmoid Activation - Sparse Cross-Entropy Loss:**
- **Shallow Model**: Akurasi = 97.25%
- **Medium Model**: Akurasi = 98.48%
- **Deep Model**: Akurasi = 98.31%

### **💡 Sigmoid Activation - Hinge Loss:**
- **Shallow Model**: Akurasi = 97.07%
- **Medium Model**: Akurasi = 98.05%
- **Deep Model**: Akurasi = 97.90%

### **💡 Tanh Activation - Cross-Entropy Loss:**
- **Shallow Model**: Akurasi = 97.26%
- **Medium Model**: Akurasi = 97.60%
- **Deep Model**: Akurasi = 97.39%

### **💡 Tanh Activation - Sparse Cross-Entropy Loss:**
- **Shallow Model**: Akurasi = 97.41%
- **Medium Model**: Akurasi = 97.55%
- **Deep Model**: Akurasi = 97.30%

### **💡 Tanh Activation - Hinge Loss:**
- **Shallow Model**: Akurasi = 96.66%
- **Medium Model**: Akurasi = 96.59%
- **Deep Model**: Akurasi = 96.68%

## 🏅 **Hasil Terbaik:**
**Deep Model dengan ReLU Activation dan Sparse Cross-Entropy Loss** mencapai **Akurasi 98.48%**, yang merupakan hasil terbaik dalam eksperimen ini! 🚀

## 🚀 **Kesimpulan:**
Eksperimen ini menunjukkan bagaimana kombinasi berbagai arsitektur, fungsi aktivasi, dan fungsi loss dapat memengaruhi kinerja model dalam klasifikasi dataset MNIST. Dengan **Deep Model** dan **ReLU Activation** serta **Sparse Cross-Entropy Loss**, model menunjukkan performa terbaik, mencapai akurasi **98.48%**!

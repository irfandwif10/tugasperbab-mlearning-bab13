# tugasperbab-mlearning-bab13
## 13. Praktikum Bab 13: Convolutional Neural Network (CNN) & Transfer Learning

### 1. CNN Sederhana dari Nol (Praktikum 1):
- **Arsitektur:** Terdiri dari lapisan konvolusi (`Conv2D`) untuk ekstraksi fitur visual dan *pooling* untuk mereduksi dimensi sebelum diklasifikasikan oleh *Dense layer*.
- **Karakteristik:** Membutuhkan waktu pelatihan yang lebih lama dan data yang banyak karena seluruh bobot jaringan dipelajari dari awal (*scratch*).

### 2. Transfer Learning dengan MobileNetV2 (Praktikum 2):
- **Feature Extraction:** Bobot *base model* dibekukan (`trainable = False`) sehingga pelatihan berlangsung jauh lebih cepat karena hanya melatih lapisan klasifikasi bagian atas[cite: 14].
- **Fine-Tuning (Opsional):** Jika akurasi dirasa kurang optimal, beberapa *layer* terakhir dari *base model* dapat dicairkan (*unfreeze*) dan dilatih ulang menggunakan *learning rate* yang sangat kecil (misal $1e-5$)[cite: 14].

🐋 Ensemble Citra Berbasis Spectral Contrast untuk Klasifikasi Spesies Mamalia Laut

Data Mining Intelecta 2025

Proyek ini berfokus pada klasifikasi 32 spesies mamalia laut berdasarkan vokalisasi akustik menggunakan pendekatan berbasis citra. Dengan memanfaatkan spectral contrast sebagai fitur utama serta arsitektur deep learning berbasis gambar, penelitian ini bertujuan meningkatkan akurasi identifikasi spesies yang sulit dideteksi oleh pendengaran manusia.

Pendekatan ini menggabungkan teknik ekstraksi fitur audio, transformasi citra, dan ensemble model citra modern.

📌 Latar Belakang

Identifikasi mamalia laut melalui vokalisasi menjadi penting karena:

Mereka memiliki peran ekologis penting.

Setiap spesies memiliki ciri akustik unik, namun sering berada pada frekuensi yang sulit didengar manusia.

Ketersediaan data vokalisasi terbatas membuat model harus robust terhadap variasi suara.

Pendekatan berbasis citra spektral memungkinkan model menangkap pola frekuensi yang tidak mudah terlihat dari audio mentah.

🎯 Tujuan Penelitian

Mengekstraksi ciri khas vokalisasi mamalia laut menggunakan spectral contrast.

Mengonversi fitur tersebut menjadi citra 2D untuk analisis visual berbasis CNN.

Membangun dan membandingkan performa tiga model citra:

WhaleNet

ResNet-50

VGG-16

Mengembangkan ensemble model untuk meningkatkan generalisasi dan akurasi.

🧠 Metodologi
1. Ekstraksi Fitur – Spectral Contrast

Mengukur kontras intensitas antara puncak (peaks) dan lembah (valleys) spektral.

Menonjolkan pola frekuensi yang unik pada tiap spesies.

Kontras-spektral → direpresentasikan sebagai citra 2D.

2. Arsitektur Model

Tiga model CNN digunakan:

Model	Deskripsi
WhaleNet	Model khusus vokalisasi laut, paling unggul pada studi ini
ResNet-50	Deep CNN dengan residual blocks
VGG-16	CNN berlapis dalam, populer untuk citra sederhana
3. Ensemble Learning

Menggabungkan prediksi ketiga model.

Menangkap variasi pola spektral yang berbeda.

Memberikan peningkatan signifikan pada performa.

📈 Hasil Eksperimen
Model	F1-Macro
WhaleNet + Spectral Contrast	0.9635
ResNet-50	(nilai sesuai makalah, jika ada)
VGG-16	(nilai sesuai makalah)
Ensemble Model	0.9857

✨ Ensemble menghasilkan peningkatan performa tertinggi, menunjukkan bahwa variasi pola yang ditangkap tiap model saling melengkapi.

🧩 Kontribusi Utama

Membuktikan bahwa spectral contrast adalah fitur efektif untuk vokalisasi mamalia laut.

Menunjukkan bahwa pendekatan citra (bukan audio langsung) memberikan kinerja tinggi.

Menghasilkan ensemble model dengan akurasi mendekati sempurna (F1 0.9857).

Menghadirkan pipeline yang tetap kuat meski dataset vokalisasi relatif terbatas.

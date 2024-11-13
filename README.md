<h1 align="center">🌟 Creating anime characters using Deep Convolutional Generative Adversarial Networks (DCGANs) and Keras 🌟</h1>
<p align="center">🔍 Create Gambar anime from DCGANs dan Keras! 🔍</p>

<div align="center">
    <img src="https://img.shields.io/badge/Jupyter-FFAA00?style=for-the-badge&logo=Jupyter&logoColor=white">
    <img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54">
    <img src="https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white">
    <img src="https://img.shields.io/badge/Infinite_Learning-4B0082?style=for-the-badge&logo=book&logoColor=white">
    <img src="https://img.shields.io/badge/Google_Drive-34A853?style=for-the-badge&logo=googledrive&logoColor=white">
    <img src="https://img.shields.io/badge/DCGANs-FF5722?style=for-the-badge&logo=huggingface&logoColor=white">
    <img src="https://img.shields.io/badge/Keras-008080?style=for-the-badge&logo=caikit&logoColor=white">
</div>

## 🎯 Gambaran Proyek

Proyek ini menunjukkan cara menggunakan Deep Convolutional Generative Adversarial Networks (DCGANs) dengan Keras untuk menghasilkan karakter bergaya anime. Dengan memanfaatkan arsitektur GAN, kita dapat membuat gambar karakter baru yang mengikuti pola statistik dari dataset pelatihan. Proyek ini dapat diperluas untuk aplikasi pengembangan video game, animasi, atau desain karakter.

Notebook ini dirancang untuk dijalankan di Google Colab, yang menyediakan sumber daya komputasi, termasuk dukungan GPU, untuk mempercepat proses pelatihan dan menghasilkan hasil lebih cepat.

Teknologi yang Digunakan

- Python: Bahasa pemrograman utama yang digunakan untuk mengimplementasikan model deep learning.
  
- Keras: API deep learning tingkat tinggi yang memudahkan pembuatan dan pelatihan model GAN.
  
- TensorFlow: Menyediakan backend komputasi untuk Keras, dengan kemampuan akselerasi GPU yang mempercepat pelatihan model.
  
- NumPy: Digunakan untuk manipulasi data, terutama dalam pemuatan dan pemrosesan data gambar.
  
- Matplotlib: Library visualisasi yang digunakan untuk menampilkan contoh karakter yang dihasilkan, membantu memantau kemajuan model.
  
- Google Colab: Platform berbasis cloud yang memungkinkan pengguna melatih model deep learning dengan GPU gratis, sehingga lebih mudah diakses dan efisien untuk tugas yang memerlukan sumber daya besar

## 🚀 Arsitektur DCGAN dan Alur Kerja

#### **Model Generator dan Discriminator**
- **Generator:** Mengambil input berupa noise acak dan menghasilkan gambar yang mencoba meniru tampilan data pelatihan.
- **Discriminator:** Sebuah klasifikator yang membedakan antara gambar asli (dari data pelatihan) dan gambar palsu (dari generator).

Kedua model dilatih dalam kerangka kompetitif di mana generator terus meningkatkan hasilnya berdasarkan umpan balik dari discriminator, menghasilkan gambar yang semakin realistis seiring waktu.
  
#### **Proses Pelatihan**
- **Persiapan Data:** Dataset yang digunakan dalam proyek ini terdiri dari berbagai gambar karakter anime, yang membantu model mempelajari elemen-elemen penting seperti gaya dan struktur.
  
- **Pelatihan:** Kedua model dilatih secara iteratif. Discriminator mencoba memperbaiki kemampuan membedakan gambar asli dari yang palsu, sementara generator belajar membuat gambar yang bisa "menipu" discriminator.
  
- **Penyimpanan dan Hasil:** Selama proses pelatihan, notebook menyimpan dan menampilkan gambar hasil generator pada interval tertentu untuk menunjukkan peningkatan model.

#### **Hasil**
![image](https://github.com/user-attachments/assets/eb110a57-aa91-4231-9b08-3847af92b408)
![image](https://github.com/user-attachments/assets/9e86b810-5282-4bd8-bcf7-14f7405259a1)


## 📝 Analisis Teknologi yang Digunakan

#### **Mengapa Menggunakan DCGAN untuk Generasi Gambar?**
- GAN dipilih karena kemampuannya menghasilkan gambar baru yang terlihat realistis dan mengikuti distribusi statistik dari data input. Dengan menggabungkan layer konvolusi, DCGAN mampu mengekstraksi fitur hierarkis, yang meningkatkan kemampuan dalam menghasilkan gambar yang koheren secara visual dengan menangkap fitur lokal dan global pada data. Arsitektur ini ideal untuk menghasilkan gambar, terutama ketika dataset memiliki gaya yang jelas, seperti karakter anime.

#### **Mengapa Keras dengan TensorFlow?**
- Keras menyediakan antarmuka tingkat tinggi yang menyederhanakan pembuatan model deep learning yang kompleks, sehingga mempercepat eksperimen dengan arsitektur model. Ini sangat cocok untuk DCGAN karena strukturnya yang modular memungkinkan konfigurasi generator dan discriminator dengan mudah. TensorFlow menyediakan dukungan GPU, yang sangat penting untuk melatih DCGAN dengan efisien. Kombinasi Keras dan TensorFlow adalah pilihan ideal untuk tugas yang memerlukan banyak sumber daya seperti generasi gambar.

#### **Mengapa Google Colab?**
- Google Colab menyediakan akses ke GPU gratis, sehingga dapat diakses oleh pengembang dan peneliti yang bekerja pada proyek deep learning tanpa perlu perangkat keras yang mahal. Colab juga memungkinkan berbagi notebook dengan mudah, memfasilitasi kolaborasi dan reprodusibilitas hasil. Dalam kasus ini, Colab sangat berguna karena menyediakan sumber daya yang diperlukan untuk menjalankan DCGAN, yang membutuhkan komputasi yang intensif.

## 📌 Kesimpulan
Proyek ini berhasil menunjukkan bagaimana DCGAN dapat digunakan untuk menghasilkan karakter anime baru yang realistis. DCGAN mampu menangkap detail-detail gaya dari data pelatihan dan menghasilkan gambar yang mirip dengan data tersebut. Dengan menggunakan Keras dan TensorFlow di Google Colab, proyek ini tidak hanya efisien tetapi juga terjangkau dan mudah diakses. Teknologi ini membuka peluang besar untuk berbagai industri yang memerlukan konten unik dan dapat diskalakan, seperti pengembangan video game, animasi, dan desain karakter. Melalui DCGAN, kita bisa mencapai generasi karakter unik dalam skala besar, yang sangat bermanfaat untuk aplikasi di masa depan.

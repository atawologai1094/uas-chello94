# uas-chello94
NAMA : MARSELINUS KAKI WODA
<br>
NIM  : 181011402269
<br>
KLS  :06TPLE023
<br>
<br>
  Random forest (RF) adalah suatu algoritma yang digunakan pada klasifikasi data dalam jumlah yang besar. Klasifikasi random forest dilakukan melalui penggabungan pohon (tree) dengan melakukan training pada sampel data yang dimiliki. Penggunaan pohon (tree) yang semakin banyak akan mempengaruhi akurasi yang akan didapatkan menjadi lebih baik. Penentuan klasifikasi dengan random forest diambil berdasarkan hasil voting dari tree yang terbentuk. Pemenang dari tree yang terbentuk ditentukan dengan vote terbanyak. Pembangunan pohon (tree) pada random forest sampai dengan mencapai ukuran maksimum dari pohon data. Akan tetapi,pembangunan pohon random forest tidak dilakukan pemangkasan (pruning) yang merupakan sebuah metode untuk mengurangi kompleksitas ruang. Pembangunan dilakukan dengan penerapan metode random feature selection untuk meminimalisir kesalahan. Pembentukan pohon (tree) dengan sample data menggunakan variable yang diambil secara acak dan menjalankan klasifikasi pada semua tree yang terbentuk. Random forest menggunakan Decision Tree untuk melakukan proses seleksi. Pohon yang dibangun dibagi secara rekursif dari data pada kelas yang sama. Pemecahan (split) digunakan untuk membagi data berdasarkan jenis atribut yang digunakan. Pembuatan decision tree pada saat penentuan klasifikasi,pohon yang buruk akan membuat prediksi acak yang saling bertentangan. Sehingga,beberapa decision tree akan menghasilkan jawaban yang baik. Random forest merupakan salah satu cara penerapan dari pendekatan diskriminasi stokastik pada klasifikasi. Proses Klasifikasi akan berjalan jika semua tree telah terbentuk.Pada saat proses klasifikasi selesai dilakukan, inisialisasi dilakukan dengan sebanyak data berdasarkan nilai akurasinya. 
  <br>
  <br>
  Keuntungan penggunaan random forest yaitu mampu mengklasifiksi data yang memiliki atribut yang tidak lengkap,dapat digunakan untuk klasifikasi dan regresi akan tetapi tidak terlalu bagus untuk regresi, lebih cocok untuk pengklasifikasian data serta dapat digunakan untuk menangani data sampel yang banyak. Proses klasifikasi pada random forest berawal dari memecah data sampel yang ada kedalam decision tree secara acak. Setelah pohon terbentuk,maka akan dilakukan voting pada setiap kelas dari data sampel. Kemudian, mengkombinasikan vote dari setiap kelas kemudian diambil vote yang paling banyak.Dengan menggunakan random forest pada klasifikasi data maka, akan menghasilkan vote yang paling baik. 
  <br>
  <br>
  Sejarah Metode umum dari random decision forest pertama kali diusulkan oleh Ho pada tahun 1995,Tin Kam Ho yang menetapkan bahwa pohon-pohon keputusan di random forest membelah diri dengan hyperplanes yang miring, jika secara acak dibatasi untuk peka hanya pada dimensi fitur yang dipilih, maka dapat memperoleh akurasi ketika pohon-pohon keputusan tumbuh tanpa terlalu banyak berlatih.Sebuah karya berikutnya  pada tema yang sama  menyimpulkan bahwa metode pemisahan lain, selama pohon-pohon keputusan secara acak dipaksa tidak peka terhadap beberapa dimensi fitur, berperilaku sama. Perhatikan bahwa pengamatan terhadap pengklasifikasi yang lebih kompleks (hutan yang lebih besar) yang semakin akurat hampir secara monoton sangat kontras dengan keyakinan umum bahwa kompleksitas penggolongan hanya dapat tumbuh pada tingkat akurasi tertentu sebelum disakiti dengan overfitting. Penjelasan tentang perlawanan metode hutan terhadap overtraining dapat ditemukan dalam teori Kleinberg tentang diskriminasi stokastik. Awal mula perkembangan gagasan Breiman tentang random forest dipengaruhi oleh karya Amit dan Geman  yang memperk enalkan gagasan pencarian lebih dari satu subset acak dari keputusan yang tersedia ketika memisahkan sebuah simpul, dalam konteks menumbuhkan satu pohon. Gagasan pemilihan subruang acak dari Ho juga berpengaruh dalam desain random forest. Dalam metode ini, hutan pepohonan ditanam, dan variasi di antara pepohonan diperkenalkan dengan memproyeksikan data pelatihan ke dalam subruang yang dipilih secara acak, sebelum memasang setiap pohon atau setiap simpul. Kemudian, jadilah ide pengoptimalan node acak, di mana keputusan di setiap node dipilih dengan prosedur acak, dari optimasi deterministik yang pertama kali diperkenalkan oleh Dietterich. 
  <br>
  <br>
  Random forest pertama kali di publikasikan dengan beberapa persiapan ialah melalui makalah oleh Leo Breiman Makalah ini menjelaskan metode membangun hutan pohon yang tidak berkorelasi menggunakan prosedur seperti CART (Classification And Regression Trees), dikombinasikan dengan pengoptimalan simpul acak dan bagging. Selain itu, makalah ini menggabungkan beberapa bahan, beberapa sebelumnya dikenal dan beberapa novel, yang membentuk dasar dari praktik modern hutan acak, 
  <br>
  khususnya: 
- 1. Menggunakan out-of-bag error sebagai perkiraan kesalahan generalisasi. 
- 2. Mengukur variabel penting melalui permutasi. 
  <br>
  Laporan ini juga menawarkan hasil teoretis pertama untuk random forest dalam bentuk batas pada kesalahan generalisasi yang tergantung pada kekuatan pohon di hutan dan korelasinya.  
  <br>
```javascript 
Contoh  : import numpy as np from sklearn import preprocessing from sklearn.ensemble import RandomForestClassifier import matplotlib.pyplot as plt 
```

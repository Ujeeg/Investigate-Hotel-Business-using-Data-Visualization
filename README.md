# Investigate-Hotel-Business-using-Data-Visualization

Sangat penting bagi suatu perusahaan untuk selalu menganalisa performa bisnisnya. Pada kesempatan kali ini, kita akan lebih mendalami bisnis dalam bidang perhotelan. Fokus yang kita tuju adalah untuk mengetahui bagaimana perilaku pelanggan kita dalam melakukan pemesanan hotel, dan hubungannya terhadap tingkat pembatalan pemesanan hotel. Hasil dari insight yang kita temukan akan kita sajikan dalam bentuk data visualisasi agar lebih mudah dipahami dan bersifat lebih persuasif.

## Data Prepocessing
1. Melakukan pengecekan data menggunakan data null 
   Didapat 4 coloumn dengan null yaitu city, agent, company, dan children dilakukan pengisian data null

2. Melakukan pengisian data NULL
   - Children null bisa di anggap menjadi 0
   - City yang null menggunakan logika Tidak dikenal (Unknown) lalu di isi dengan Unknown
   - Agent yang null di anggap tidak menggunakan agent dengan logika True/False lalu di isi 0
   - Company yang null di anggap tidak menggunakan agent jadi di isi 0

3. Merubah data yang keliru pada Kolom Meal (mengganti ‘Undefined menjadi No Meal’)

4. Menseleksi atau drop kolom data yang tidak di perlukan

Code Source
https://drive.google.com/file/d/1Dpww2MqYyVKUo9KGcACKOHB7GtQCt1DJ/view?usp=share_link



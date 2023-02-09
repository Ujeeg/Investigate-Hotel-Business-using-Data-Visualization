# Investigate-Hotel-Business-using-Data-Visualization

Sangat penting bagi suatu perusahaan untuk selalu menganalisa performa bisnisnya. Pada kesempatan kali ini, kita akan lebih mendalami bisnis dalam bidang perhotelan. Fokus yang kita tuju adalah untuk mengetahui bagaimana perilaku pelanggan kita dalam melakukan pemesanan hotel, dan hubungannya terhadap tingkat pembatalan pemesanan hotel. Hasil dari insight yang kita temukan akan kita sajikan dalam bentuk data visualisasi agar lebih mudah dipahami dan bersifat lebih persuasif.

## Data Prepocessing
1. Melakukan pengecekan data menggunakan data null 
   Didapat 4 coloumn dengan null yaitu city, agent, company, dan children dilakukan pengisian data null
   
![Null sum](https://user-images.githubusercontent.com/118154539/217796954-1f7ffc83-9be5-42e4-8e46-5ab46c0fab1b.png)


2. Melakukan pengisian data NULL
   - Children null bisa di anggap menjadi 0
   - City yang null menggunakan logika Tidak dikenal (Unknown) lalu di isi dengan Unknown
   - Agent yang null di anggap tidak menggunakan agent dengan logika True/False lalu di isi 0
   - Company yang null di anggap tidak menggunakan agent jadi di isi 0
       ![fill null](https://user-images.githubusercontent.com/118154539/217796979-8708923d-75eb-45a6-aecf-9b55463917e7.png)

3. Merubah data yang keliru pada Kolom Meal (mengganti ‘Undefined menjadi No Meal’)
     - pengecekan Meal value
 
       ![meal value](https://user-images.githubusercontent.com/118154539/217797571-b7cd8013-1d33-4c7d-87a4-830634b9d13f.png)
      
    - merubah value meal undefinied ke No meal
   
       ![meal change valuw](https://user-images.githubusercontent.com/118154539/217797732-5646692a-5844-4211-b8a1-2cf7848ee1d0.png)


4. Menseleksi atau drop kolom data yang tidak di perlukan
  - Membuat kolom data baru dengan menggabungkan data adult, children, babies menjadi visitor
  - Membuat kolom data baru dengan menggabungkan data_stay_in_weekend_night dan stay_in_weekdays_night menjadi stay duratin
     ![Visitor stay duration](https://user-images.githubusercontent.com/118154539/217798945-a15de9d7-db1b-4d31-a6e2-d603d77fbccc.png)

  - Menseleksi data
     ![selection data](https://user-images.githubusercontent.com/118154539/217799040-42e53673-bbf2-47e0-b214-a04a0a047f72.png)
 


Code Source
https://github.com/Ujeeg/Investigate-Hotel-Business-using-Data-Visualization/blob/main/Project%202%20Stage%201.ipynb




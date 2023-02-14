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

3. Membuat Box Pot untuk menghilangkan Ouliers
      ![outliers barplot](https://user-images.githubusercontent.com/118154539/218632591-28d4ea9b-7896-489e-bc89-a029c31b4594.png)

4. Membersihkan Outliers dengan Zscore
      ![Cleaning ouliers](https://user-images.githubusercontent.com/118154539/218632686-de990adf-a660-419f-a6af-16bdbc5c1a30.png)

5. Merubah data yang keliru pada Kolom Meal (mengganti ‘Undefined menjadi No Meal’)
     - pengecekan Meal value
 
       ![meal value](https://user-images.githubusercontent.com/118154539/217797571-b7cd8013-1d33-4c7d-87a4-830634b9d13f.png)
      
    - merubah value meal undefinied ke No meal
   
       ![meal change valuw](https://user-images.githubusercontent.com/118154539/217797732-5646692a-5844-4211-b8a1-2cf7848ee1d0.png)


6. Menseleksi atau drop kolom data yang tidak di perlukan
  - Membuat kolom data baru dengan menggabungkan data adult, children, babies menjadi visitor
  - Membuat kolom data baru dengan menggabungkan data_stay_in_weekend_night dan stay_in_weekdays_night menjadi stay duratin
     ![Visitor stay duration](https://user-images.githubusercontent.com/118154539/217798945-a15de9d7-db1b-4d31-a6e2-d603d77fbccc.png)

  - Menseleksi data
     ![selection data](https://user-images.githubusercontent.com/118154539/217799040-42e53673-bbf2-47e0-b214-a04a0a047f72.png)
 
# Montly Hotel Booking Analysis Based on Hotel Type
1. Mothly Hotel Booking Analysis Based on Hotel Type and Month
![stage 2 1](https://user-images.githubusercontent.com/118154539/218632920-16eb60fd-ab28-4d3b-8db0-d85477f925e9.png)
Pada plot Montly Hotel Booking Analysis Based on Hotel Type didapat bahwa :
   1) Dari data di atas dapat di lihat bahwa nilai booking City hotel lebih tinnggi di bandung resort hotel
   2) Untuk data per month pada city hotel bisa di lihat bahwa pada bulan july dan Agustus
   3) Untuk data per month pada Resort Hotel bisa di lihat bahwa pada bulan july dan December

2. Yearly Hotel Booking Analysis Based on Hotel Type
![stage 2 2](https://user-images.githubusercontent.com/118154539/218633167-7959cd59-3e3a-4881-b4a2-e9c7a8f93845.png)
Dari data dapat di lihat bahwa tiap tahunnya terjadi kenaikan, kenaikan yang cukup signifikan dari tahun 2017 ke 2018

# Impact Analysis of Stay Duration on Hotel Bookings Cancellation
1. Analysis of Stay Duration on Hotel Bookings Cancellation
![Plot cannceled](https://user-images.githubusercontent.com/118154539/218633318-d9abd04a-6a67-485d-b37d-b510295f36bb.png)
Pada plot Analysis of Stay Duration on Hotel Bookings Cancellation didapat bahwa :
   1) Dari data di atas dapat dilihat bahwa tingkat canceled tidak lebih tinggi dibanding not canceled
   2) Tingkat canceled paling tinggi terjadi pada durasi 2-3 stay duration

2. Impact Analysis of Month on Hotel Bookings Cancellation
![Plot cannceled](https://user-images.githubusercontent.com/118154539/218633450-59d8cddf-adf4-4afc-81d7-71ad7f0fe7d7.png)

Pada plot Analysis of Stay duration on Booking Cancellation didapat bahwa  :
Tingkat canceled tidak lebih besar dari not canceled
Pada stay duration 1 dan 3 terdapat tingkat canceled dan not canceled paling tinggi
Untuk tingkat canceled pada stay duration 1 jauh lebih rendah dibanding dengan stay duration 2 dan 3, hal tersebut bisa saja terjadi karena pengunjung merasa kecewa dengan hotel/ tidak sesuai ekspektasi, dan menyebabkan pengunjung memilih untuk pindah ke hotel lain di stay duration 2 dan 3 
Di dapat bahwa semakin lama stay duration semakin sedikit juga tingkat bookingnya
Pada stay 1,2 dan 3 merupakan lama stay duration paling di minati pengunjung, mungkin dengan ini hotel bisa membuat promo untuk stay duration 2-3, antau mungkin bisa menggunaka logika untuk meningkatkan stay duration dengan memberikan promo khusus pada pengunjung yang melakukan booking lebih dari 3 stay duration 
![image](https://user-images.githubusercontent.com/118154539/218633522-06b3a6c1-c181-4201-9c0d-ea4b8344683d.png)

3. Analysis of Hotel Type on Hotel Bookings Cancellation
![Plot cannceled 3](https://user-images.githubusercontent.com/118154539/218633965-37a011d9-8e08-467c-ad04-7970df8cc088.png)
Pada plot Analysis of Hotel Type on Hotel Bookings Cancellation didapat bahwa  :

Di dapat bahwa tingkat Booking pada resort hotel lebih tinngi di banding city hotel dengan stay duration yang cukup tinggi
Tingkat canceled terjadi di atas 3 stay duration pada resort hotel dan pada city hotel rata –rata pengunjung melakukan cancel di durasi stay duration 2 ke atas 
![image](https://user-images.githubusercontent.com/118154539/218633994-15bf8ac6-af0b-41c7-9072-69f4799f4d4c.png)

# Impact Analysis of Lead Time on Hotel Bookings Cancellation Rate
1. Impact Analysis of Lead Time on Hotel Bookings Cancellation 
![Stage 3](https://user-images.githubusercontent.com/118154539/218634110-f8c3ebf6-d6d9-416a-b9bc-295982412d13.png)
Pada Data Impact Analysis of Lead Time on Hotel Bookings Cancellation dapat di lihat bahwa :
   1) Tingkan cancel terjad pada lead time di atas 70
   2)Lama booking hotel pada resort hotel dan city hotel yang not canceled hampir sama dimana lead time paling lama ada di bawah 70 lead time

2.  Analysis of Lead Time on Hotel Bookings Cancellation by Hotel Type
![Stage 3 1](https://user-images.githubusercontent.com/118154539/218634420-ef2b9df3-0152-4ed2-a78d-c4942413a547.png)
Pada Data Impact Analysis of Lead Time on Hotel Bookings Cancellation by Hotel Type dapat di lihat bahwa :
   1) Tingkan cancel terjadi pada interval di atas 70 untuk Resort hotel
   2) Tingkan cancel terjadi pada interval di atas 80 untuk Resort hotel
   3)lama booking hotel pada resort hotel dan city hotel yang not canceled hampir sama dimana lead time paling lama ada di bawah 80 lead time

3. Analysis of Stay Duration on Hotel Bookings Cancellation by Month
![Stge 3 2](https://user-images.githubusercontent.com/118154539/218634290-d01711ce-2883-4d52-850f-56bd06e33e3f.png)
   1) Canceled dangan lead time paling lama terjadi pada bulan November, hal tersebut bisa terjadi karena banya pengunjung yang merencanakan untuk melakukan booking pada bulan December dimana terdapat libur panjang yaitu libur natal dan tahun baru
   2)canceled dengan lead time paling singkat terjadi pada bulan April
Code Source
https://github.com/Ujeeg/Investigate-Hotel-Business-using-Data-Visualization/blob/main/Project%202%20Stage%201.ipynb




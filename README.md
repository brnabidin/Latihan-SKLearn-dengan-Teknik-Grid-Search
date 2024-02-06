# Latihan-SKLearn-dengan-Teknik-Grid-Search

**Tahapan Latihan**

Tahapan latihan kali ini sebagai berikut:

- Ubah dataset data menjadi Dataframe.

- Definisikan parameter yang akan diuji.

- Jalankan fungsi grid search.

- Latih model dengan parameter terbaik hasil grid search.

- Buat plot dari model.

# Codelab

Pertama, unduh berkas "Salary_Data.csv", dari tautan "https://www.kaggle.com/vivinbarath/simple-linear-regression-for-salary-data/data" berikut ini. Jika sudah jangan lupa upload ke Google Colab Anda. Berikut caranya.

![1](https://github.com/brnabidin/Latihan-SKLearn-dengan-Teknik-Grid-Search/assets/67081096/09662448-b561-4de3-a486-85f2e220bad6)

Kemudian pisahkan atribut dan label pada dataset. Masih ingat bukan, bahwa jika hanya terdapat 1 atribut pada dataset kita perlu mengubah bentuknya agar bisa dipakai pada pelatihan model.

![2](https://github.com/brnabidin/Latihan-SKLearn-dengan-Teknik-Grid-Search/assets/67081096/5b9566d2-c9d2-4fbb-9bca-a2b9ba05230d)

Selanjutnya, untuk menggunakan grid search, kita impor library GridSearchCV dari sklearn.model_selection. Lalu kita buat model yang ingin kita uji dengan grid search dalam hal ini model SVR. Kemudian kita buat sebuah python dictionary yang berisi nama parameter yang akan diuji, serta nilai-nilainya. Selanjutnya kita buat objek grid search dan mengisi parameter-parameternya. Parameter pertama adalah model yang akan kita uji. Parameter kedua adalah dictionary yang berisi kumpulan parameter dari model yang akan diuji. Terakhir kita panggil fungsi fit() pada objek grid search yang telah kita buat.

![3](https://github.com/brnabidin/Latihan-SKLearn-dengan-Teknik-Grid-Search/assets/67081096/5660bffe-8c65-44df-b1c9-123959961024)

Setelah grid search mencari parameter terbaik pada model, kita bisa menampilkan parameter terbaik dengan memanggil atribut best_params_ dari objek grid search.

![4](https://github.com/brnabidin/Latihan-SKLearn-dengan-Teknik-Grid-Search/assets/67081096/485bf564-c117-449b-93d6-0fd521821cfd)

Selanjutnya Anda bisa mencoba membuat model SVM baru dengan parameter hasil grid search dan melatihnya pada data.

![5](https://github.com/brnabidin/Latihan-SKLearn-dengan-Teknik-Grid-Search/assets/67081096/464df151-9c82-4223-b8b8-e574f9f31705)

Terakhir kita bisa memvisualisasikan SVR dengan parameter hasil grid search. Dapat dilihat dari hasil plot bahwa grid search berhasil mencari parameter yang lebih baik sehingga meningkatkan performa dari model.

![6](https://github.com/brnabidin/Latihan-SKLearn-dengan-Teknik-Grid-Search/assets/67081096/f6f27960-31d2-4699-a5d5-5cd64c60c68a)

![20200430175750c0258f1d2bdc64a9fd8bf76dda6d50cb](https://github.com/brnabidin/Latihan-SKLearn-dengan-Teknik-Grid-Search/assets/67081096/57c0bd72-d471-4303-aea6-2bf1e8845e9c)

# ml_process_company_bankruptcy_prediction

Lembaga keuangan perlu memprediksi kebangkrutan perusahaan agar mereka dapat membuat keputusan pinjaman yang tepat. Sehingga dapat dipastikan bahwa perusahaan yang meminjam uang dari mereka tidak akan mengalami kesulitan keuangan atau bahkan bangkrut. 
Selain itu, lembaga keuangan dapat menghindari risiko lebih besar dan dapat mempertahankan reputasi baik di mata masyarakat dan nasabah.

Terdapat tiga model yang digunakan dalam pemodelan ini yaitu K-Nearest Neighbors (KNN), Logistic Regression, dan Random Forest.

Data yang digunakan dalam pemodelan ini mengalami ketidakseimbangan.

Proses pemodelan terdiri dari dua percobaan, yaitu dengan data yang tidak seimbang (Percobaan 1) dan dengan data yang telah diimbangi menggunakan SMOTENC (Percobaan 2).

Prediksi kebangkrutan memiliki konsekuensi finansial atau hukum yang sangat besar (misalnya, dalam pengambilan keputusan investasi atau pemberian pinjaman), maka harus meminimalkan false negatives (mengidentifikasi perusahaan yang sebenarnya bangkrut sebagai tidak bangkrut). Dalam hal ini, recall menjadi metrik yang paling penting. Sehingga LogReg Resampled menjadi model terpilih.

Dari pemodelan yang dilakukan, tidak ada model yang melebihi baseline accuracy (96%) di data test. Namun, model tetap dapat digunakan karena mendapatkan hasil recall yang cukup baik (50%). Sehingga dapat meminimalkan 50% kesalahan memprediksi perusahaan yang sebenarnya bankrut sebagai tidak bankrut.

Penggunaan SMOTENC untuk menyeimbangkan data train terbukti menaikkan nilai recall pada model KNN, Logistic Regression dan Random Forest. Setelah pemilihan model, model Logistic Regression memiliki performa yang baik dengan data train yang asli.

# Capstone3__TelcoCustomerChurn_IntanPermatasari
# **BUSINESS UNDERSTANDING**
**Context:**

Industri telekomunikasi berkembang pesat dengan persaingan ketat antar perusahaan yang menawarkan layanan berlangganan. Tantangan utama perusahaan adalah mempertahankan pelanggan agar tidak beralih ke kompetitor. 

Sebuah perusahaan ingin mengidentifikasi pelanggan yang berpotensi berhenti berlangganan (churn) untuk mengurangi angka churn. Data Scientist diminta membuat model prediksi menggunakan Machine Learning untuk menentukan apakah pelanggan akan berhenti menggunakan layanan (churn) atau tidak.

**Target:**
- 0: Tidak berhenti menggunakan layanan
- 1: Berhenti menggunakan layanan (churn)
- **PROBLEM STATEMENT :**

Perusahaan telekomunikasi cenderung fokus pada mempertahankan pelanggan karena biaya mempertahankan pelanggan (customer retention cost) lebih rendah dibandingkan dengan biaya memperoleh pelanggan baru (customer acquisition cost). Berdasarkan data dari internet, biaya untuk mendapatkan pelanggan baru bisa mencapai lima kali lipat dari biaya untuk mempertahankan pelanggan yang sudah ada. hal ini juga dinyatakan di salah satu statistik bisnis yang terkenal yang dimana  "Biaya untuk mempertahankan pelanggan yang ada jauh lebih rendah daripada biaya untuk memperoleh pelanggan baru". Selain itu,pada [Customer Acquisition Vs. Retention Costs – Statistics And Trends](https://www.invespcro.com/blog/customer-acquisition-retention/) dikatakan bahwa biaya untuk memperoleh pelanggan baru lima kali lebih tinggi daripada biaya untuk mempertahankan pelanggan yang ada.

Untuk suatu perusahaan telekomunikasi, tingginya persentase pelanggan yang melakukan *churn* adalah salah satu indikator yang menjadi tingkat kegagalan suatu perusahaan tersebut, sehingga diperlukan upaya untuk mengurangi persentase pelanggan *churn* tersebut. Pada umumnya perusahaan lebih memilih untuk mempertahankan pelanggan, karena biaya untuk mempertahankan pelanggan *(customer retention cost)* lebih rendah daripada memperoleh pelanggan baru *(customer acquisition cost)*.Berdasarkan informasi dari internet, memperoleh pelanggan baru dapat menghabiskan biaya lima kali lebih banyak daripada mempertahankan pelanggan yang sudah ada. Adapun rata-rata biaya customer acquisition cost untuk industri telekomunikasi adalah sekitar $315 per new customer.

Salah satu cara perusahaan telekomunikasi mempertahankan para customernya agar tetap berlangganan atau tidak *churn*, yaitu dengan memberikan insentif retensi terhadap pelanggan. Insentif retensi yang dimaksud adalah dengan memberikan suku bunga yang menarik, memberikan paket layanan yang menarik, memberikan prioritas pelayanan dan lain-lain dalam upaya untuk mempertahankan para customer atau pelanggan perusahaan telekomunikasi tersebut. Namun, kebijakan pemberian insentif retensi belum sepenuhnya dilakukan secara efektif. Karena jika insentif retensi tersebut diberikan secara merata kepada seluruh pelanggan, maka pengeluaran biaya tersebut menjadi tidak efektif dan dapat mengurangi keuntungan apabila pelanggan tersebut memang loyal dan tidak ingin berhenti menggunakan layanan.

Salah satu strategi untuk mempertahankan pelanggan adalah dengan memberikan insentif retensi, seperti suku bunga menarik, paket layanan spesial, dan prioritas pelayanan. Namun, pemberian insentif ini harus dilakukan secara efektif. Memberikan insentif secara merata kepada semua pelanggan tidak efisien dan bisa mengurangi keuntungan, terutama jika diberikan kepada pelanggan yang sudah loyal dan tidak berencana berhenti menggunakan layanan.
**GOALS:**

Berdasarkan permasalahan di atas, perusahaan ingin memiliki kemampuan untuk memprediksi kemungkinan seorang pelanggan akan berhenti menggunakan layanan (churn) atau tidak. Dengan demikian, perusahaan dapat memfokuskan upaya retensi pada pelanggan yang terindikasi akan churn. Selain itu, perusahaan juga ingin mengidentifikasi berbagai faktor yang mempengaruhi retensi pelanggan agar dapat merancang kebijakan yang tepat sasaran untuk mengurangi churn.
# **Evaluation Metrics**
* True Positive (TP): Model memprediksi pelanggan akan berhenti berlangganan, kenyataannya berhenti berlangganan.
* True Negative (TN): Model memprediksi pelanggan tidak akan berhenti berlangganan, kenyataannya tidak berhenti berlangganan.
* False Positive (FP): Model memprediksi pelanggan akan berhenti berlangganan, kenyataannya tidak berhenti berlangganan.
* False Negative (FN): Model memprediksi pelanggan tidak akan berhenti berlangganan, kenyataannya berhenti berlangganan.

**Consequences**
* False Positive (FP): Mengira pelanggan akan berhenti berlangganan padahal tidak. Ini bisa menyebabkan perusahaan memberikan insentif atau diskon yang tidak perlu untuk mempertahankan pelanggan yang sebenarnya tidak berencana berhenti, sehingga meningkatkan biaya operasional.
* False Negative (FN): Mengira pelanggan tidak akan berhenti berlangganan padahal sebenarnya berhenti. Ini bisa mengakibatkan hilangnya pendapatan yang potensial karena perusahaan tidak melakukan tindakan preventif untuk mencegah churn pelanggan.
Confusion Matrix


Dalam konteks prediksi churn pelanggan telco, konsekuensi dari False Positive (FP) dan False Negative (FN) memiliki dampak signifikan terhadap operasional dan pendapatan perusahaan:

Perusahaan mungkin memberikan insentif atau diskon yang tidak perlu untuk mempertahankan pelanggan yang sebenarnya tidak berencana berhenti.
Ini meningkatkan biaya operasional tanpa alasan yang jelas, karena sumber daya dialokasikan untuk mengatasi churn yang sebenarnya tidak terjadi.Disamping itu perusahaan kehilangan kesempatan untuk melakukan tindakan preventif untuk mempertahankan pelanggan tersebut.
Mengakibatkan hilangnya pendapatan yang potensial, karena pelanggan yang berhenti tidak terdeteksi oleh model dan tidak diberikan upaya retensi yang tepat.

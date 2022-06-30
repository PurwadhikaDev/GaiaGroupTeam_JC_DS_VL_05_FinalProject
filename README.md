# VEHICLE INSURANCE CUSTOMER DATA

by [Abdul Kadir Syahab](https://github.com/SyahabKadir//), [Alaniah Nisrina](https://github.com/alaniahN), and [Farhan Guido Haryadi](https://github.com/farhanguidoh)

## Contents :
- [Business Understanding](#business-understanding)
- [Data Understanding](#data-understanding)
- [Exploratory Data Analysis](#Exploratory-Data-Analysis)
- [Preprocessing](#Preprocessing)
- [Methodology (Modeling/Analysis)](#Methodology-(Modeling/Analysis))
- [Conclusion and Recommendation](#Conclusion-and-Recommendation)
---

<a id="business-understanding"></a> 
## 1. Business Understanding
### Context
Sebuah perusahaan vehicle insurance yang bertempat di wialayah Amerika Serikat bagian barat ingin memprediksi customer baru yang tertarik dengan produk asuransi mereka. Dimana calon customer tersebut di-approach dengan berbagai cara oleh perusahaan. Setelah banyak calon customer yang tertarik dan ingin membeli policy yang ditawarkan oleh tim sales & marketing, ternyata beberapa calon customer baru yang tidak relavan dengan preliminary yang telah dibuat oleh perusahaan. Melihat hal ini, tentunya akan merugikan perusahaan apabila calon customer tersebut tidak mampu untuk membayar premi per bulan kedepannya. Dari hal tersebut, maka perusahaan harus menyeleksi calon customer dengan response yes dan no kepada calon customer, apakah calon customer tersebut dianggap layak untuk membeli policy atau tidak. Oleh sebab itu perusahaan ingin mengetahui calon customer yang mana yang layak dan benar-benar mampu untuk membeli policy dan membayar premi per bulannya. Hal ini dilakukan untuk menjadi sebuah efektivitas dalam memilih calon customer dimana tentunya akan mengurangi waktu yang dibutuhkan dan biaya yang dikeluarkan oleh tim marketing. Di dalam database perusahaan ini, terdapat informasi mengenai demografi, pendidikan, income customer dll.

Target :
- 0 : Response no dari perusahaan (Customer yang dianggap tidak layak membeli policy)
- 1 : Response yes dari perusahaan (Customer yang dianggap layak membeli policy)
### Problem Statement
Selama proses marketing, perusahaan menyadari bahwa sangat memakan waktu dan sumber daya jika perusahaan menargetkan semua calon customer tanpa melakukan penyaringan terlebih dahulu. Perusahaan ingin meningkatkan efisiensi marketing dengan mengetahui calon customer mana yang layak dan benar-benar mampu untuk membeli policy dan membayar premi per bulannya. Karena apabila tim sales & marketing meng-approach ke semua calon customer, maka waktu dan biaya marketing pun akan menjadi sia-sia jika berdasarkan kebijakan perusahaan calon customer yang tersebut tidak layak untuk membeli policy dan mendapatkan response no.
### Goals
Dari permasalahan diatas, perusahaan ingin mencari tahu dan memprediksi kemungkinan calon customer mana yang layak dan benar-benar mampu untuk membeli policy dan membayar premi per bulannya dan mendapatkan response yes dari perusahaan. Sehingga perusahaan dapat fokus dan teknik marketing lebih efektif sehingga profit perusahaan menjadi naik.

Selain itu, perusahaan juga ingin mengetahui faktor apa saja yang bisa menjadi preliminary calon customer untuk membeli polis yang di tawarkan dan bagaimana perilaku dari calon customer yang ingin membeli polis. Sehingga perusahaan dapat membuat rencana yang lebih baik lagi dalam mendekati dan menyeleksi calon customer yang potensial untuk membeli.
### Analytic Aproach
Dari isu yang telah digambarkan diatas, kita akan menganalisis data perusahaan yang telah ada sehingga kita dapat menemukan pola dan membedakan calon customer yang layak dan benar-benar mampu untuk membeli policy dan membayar premi per bulannya sehingga mendapatkan response yes dan no dari perusahaan.

Kemudian juga kita akan membuat machine learning dengan model klasifikasi yang akan membantu perusahaan untuk dapat memprediksi probabilitas seorang calon customer yang layak dan benar-benar mampu untuk membeli policy dan membayar premi per bulannya sehingga mendapatkan response yes dan no dari perusahaan.

<a id="data-understanding"></a> 
## 2. Data Understanding
*[Data Source : Vehicle Insurance Customer Data](https://www.kaggle.com/datasets/ranja7/vehicle-insurance-customer-data)*
- Dataset diambil dari salah satu perusahaan Vehicle Insurance di Amerika Serikat tahun 2011
- Sebagian besar fitur bersifat kategori (Nominal, Ordinary, Binary), dengan beberapa fitur mempunyai kardinalitas yang tinggi
- Terdapat 24 kolom, dimana setiap baris dari kolom tersebut merepresentasikan informasi seorang kandidat yang mempunyai tanggal efektif asuransi di tahun 2011
- Target model adalah variabel response
### Attribute Information

| Attribute | Data Type | Description |
| --- | --- | --- |
| Customer | object | Customer's unique ID |
| State | object | State of customer |
| Customer Lifetime Value | float64 | Indicator value of customer by company |
| Response | object | Company's response to Customer's claim |
| Coverage | object | Coverage of Policy |
| Education | object | Customer's education |
| Effective To Date | object | Last effective date of policy |
| EmploymentStatus | object | Customer's status employment |
| Gender | object | Customer's gender |
| Income | int64 | Customer's income |
| Location Code | object | Code of location area |
| Marital Status | object | Customer's marital status |
| Monthly Premium Auto | int64 | Monthly policy debit |
| Months Since Last Claim | int64 | Months since customer last claim |
| Months Since Policy Inception | int64 | Months since customer registered/issued |
| Number of Open Complaints | int64 | Number of open complaints by customer |
| Number of Policies | int64  |  Number of open policies by customer |
| Policy Type | object | A type of policy that customer claimed |
| Policy | object | A category of policy type that customer claimed |
| Renew Offer Type | object | Type of renewal offer |
| Sales Channel | object | Type of approach customer by company |
| Total Claim Amount | float64 | An amount of customer claimed |
| Vehicle Class | Object |  A type of class vehicle that insuranced |
| Vehicle Size | Object  | A type of size vehicle that insuranced |

<a id="Exploratory-Data-Analysis"></a> 
## 3. Exploratory Data Analysis
<img src="oictures/responses.png" alt="Distribution of Response"/><br>

<a id="Preprocessing"></a> 
## 4. Preprocessing

<a id="Methodology-(Modeling/Analysis)"></a> 
## 5. Methodology (Modeling/Analysis)

<a id="Conclusion-and-Recommendation"></a> 
## 6. Conclusion and Recommendation
### Conclusion

### Recommendation
Hal-hal yang bisa dilakukan untuk mengembangkan project dan modelnya lebih baik lagi :
- `Business` :
    - Dari sisi bisnis, tim marketing pada perusahaan bisa untuk membuat promo berdua atau bundling (paket) yang lebih oke dan ciamik, misalkan dengan membuat promo pembelian kedua discount 50%. Dimana hal ini sesuai dengan market share yang telah kita lihat sebelumnya bahwa banyak calon customer yang berstatus sudah menikah. Dengan agregasi response yes yang lebih banyak, tentunya perusahaan lebih aman untuk marketing pada lini bisnis ini.
    - Selain itu perusahaan juga dapat melakukan marketing yang lebih gencar kepada calon customer yang bertempat tinggal di wilayah suburban. Karena dari segi jumlah dan agregasi response yes, wilayah suburban sangat mendominasi di setiap wilayah bagiannya. Atau juga boleh untuk lebih melakukan marketing di wilayah urban dan rural dengan menganalisa terlebih dahulu pola calon customer yang mendapatkan response yes di wilayah ini.
    - Melihat dari persebaran penjualan polis dan agregasi response yes, perusahaan bisa untuk memfokuskan marketingnya pada polis tipe personal. Dimana perusahaan dapat membuat berbagai macam tipe pada polis personal ini
    - Untuk menambah penjualan polis tipe company, perusahaan dapat melakukan kolaborasi dengan perusahaan lain seperti bank atau perusahaan lainnya. Dengan tujuan agar karyawan pada perusahaan tersebut melakukan pembayaran premi pada perusahaan ini.
    - Perusahaan dapat mereview kembali Renew Offer Type `Offer3` dan `Offer4` karena pada persentase calon customer yang di response yes sangat sedikit. `Offer3` hanya memiliki persentase yes sebanyak 2% sedangkan `Offer4` sama sekali tidak memiliki response yes. 


- `Project Model` :
    - Mencoba algorithm ML yang lain seperti membuat clustering dari behaviour calon customer, sehingga perusahaan mudah untuk mengkategorisasikan calon customer mereka sesuai dengan variable yang ada
    - Mencoba hyperparameter tuning kembali, menggunakan teknik oversampling yang berbeda juga selain Random Over Sampling, seperti SMOTENC, dll
    - Menganalisa data model lebih lanjut yang kemungkinannya kita masih salah tebak untuk mengetahui alasannya dan karakteristiknya  sehingga dapat menyempurnakan project dan model kita kedepannya
    - Menambahkan fitur-fitur (variable-variable) baru yang kemungkinan ada korelasinya dengan dataset kita miliki. Dimana seperti yang kita tahu bahwa banyak sekali preliminary Car Insurance Company dalam mengambil keputusan untuk menerima calon nasabahnya seperti umur dari calon customer, umur kendaraan dari calon customer, driving record dari calon customer dll. Hal ini dimaksudkan untuk memastikan apakah calon customer riskan dan dirasa akan merugikan company atau tidak
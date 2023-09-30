# Konsep Big Data
menjelaskan gambaran besar tentang big data

## Big Data Flow

a. siapkan use case / permasalahan
b. cari stack teknologi yang cocok

### 1. Data Collection ( cara mendapatkan data )
    1. Sourcing SQL
    2. Pub / subsribe
    3. Queue
    4. Custom Connectors ( bikin script sendiri )
    5. web scraping ;v
    6. cari data open source (Opendata, kaggle.com )

#### Notes ::
    * saat scraping pasti ada missing values, jadi harus di persiapkan

### 2. Data Preperation ( cara menyiapkan data )
    1. filtering dan menyembunyikan data
    2. sampling

### 3. Menyimpan data
> usahakan liat jenis datanya dan ukurannya :D dan cari yang cocok databasenya untuk data yang didapat

### 4. Analisa
    1. Analisa Batch : ( dikumpulkan datanya dalam rentang waktu tertentu dan baru diproses )
        * TechStack ::
            * Hadoop Map Reduce

    2. Realtime
        * TechStack ::
            * sparkSql
            * Hive
            * Redshift AWS
            * BigQuery

### 5. Visualisasi
    * TechStack ::
        * Kibana
        * MetaBase
        * bikin sendiri :D

### 6. Reporting ( jadi nanti dikasih tau langsung status Visualisasinya )
    * TechStack ::
        * Zappier
        * Email
        * Telegram


#### Notes ::
    1. saat scraping pasti ada missing values, jadi harus di persiapkan

### sumber data
    * logs yang dihasilkan web server / web
    * data transaksional
    * media sosial
    * database
    * data sensor ( IoT stuff )

>


publish subsribe model?


cara mengadopsi Big data adalah menggunakan arsitektur Sistem terdistribusi

STudy Kasus :
E- Commerece
SIRCLO : banyak data tapi ndak tau cara prosesnya
 Data  milik  SIRCLO  ini terdapat  berbagai  macam,  mulai  dari  data  milik sales,  marketing,  support,  traffic  website,  toko,


Apache Drill is an open source distributed SQL query engine that delivers fast and secure, self-service business information SQL analytics at scale.

masalah : sulit untuk membaca data tersebut karenaketerbatasan dari infrastruktur  miliknya.  Data  milik  SIRCLO  ini terdapat  berbagai  macam,  mulai  dari  data  milik sales,  marketing,  support,  traffic  website,  toko, dll.

setiap toko SIRCLO memakai database MYsql dan banyak tapi susah untuk membacanya langsung belum dan format yang berbeda JSON, MYSQL, CSV jadi dibuuthkan app juga

Tech Stack :
1. Apache Drill ( distributed SQL query engine )
2. python
3. Rclone ( buat transfer data antar subsistem )
4. ZooKeeper ( open-source coordination service for distributed applications. orchestra )?
5. Google Drive
6. S3
7. HDFS

Permasalahan : banyak nya jenis data yang di generate oleh SIRCLO dari macam variasi data dan formatnya jadi ->

1.Data didapatkan dan diubah ke format yang mampu diproses oleh Apache Drill.
2.Data mampu dikirim dari sumber data ke HDFS
3.Apache Drill mampu melakukan query dengan data SIRCLO yang tersimpan di HDFS

jawaban : berhasil mengubah arsitektur dengan teknologi

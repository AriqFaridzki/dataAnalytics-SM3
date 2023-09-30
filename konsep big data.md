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



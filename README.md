# Netflix Movie Data Analys 

This project showcase a **modern data engineering pipeline** that transforms raw data into clean,
insightfull analytics using the **Amazon S3**, **Snowflake** and **dbt**.

## 🔧 Technologies Used

- **Amazon S3** - storage for raw csv files
- **Snowflake** - cloud data warehouse for scalable ETL
- **dbt** - for transformations, testing and documentation
- **Python** - to orchestrate

---

##🗂️ Project Architecture

1. **Raw Layer**: Mirrors original MovieLens CSVs from S3  
2. **Staging Layer**: Applies cleaning, typing, and transformations  
3. **Development Layer**: Star schema modeling with fact and dimension tables  
4. **Snapshots**: Implemented Slowly Changing Dimensions (SCD Type 2)  
5. **Tests**: Ensured data integrity using dbt tests (not null, unique, relationships)

---

## 🔹 Key Features

✅ **External Stages**: Loaded raw movie data from Amazon S3 into Snowflake  
✅ **dbt Snapshots**: Captured historical changes in dimension tables (SCD Type 2)  
✅ **Data Quality Tests**: Included unique, not-null, and relationship tests  
✅ **Layered dbt Models**:
- **RAW** — Direct mapping of S3 CSVs
- **STAGING** — Cleaned, typed, and normalized data
- **DEVELOPMENT** — Star schema (facts and dimensions)

✅ **Documentation & Lineage**: Generated via `dbt docs`  

✅ **Analysis Models**: Created summary tables and exploratory models for reporting



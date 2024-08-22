# Python-ETL

the purpose by this project is to perform an ETL process by using python to extract the data out of Kaggle website by using it API to transform the data then load it to SQL-Server database to perform an analysis.

The process of using the Kaggle API:
1) Download the API tool by the Kaggle Website to the local machine.
2) install the library and the dataset:
!pip install kaggle
import kaggle
!kaggle datasets download ankitbansal06/retail-orders -f orders.csv

The dataset would be downloaded as zip file in it will be the CSV file.

3) Unzip the file by using the ZipFile library:
import zipfile
zip_ref= zipfile.ZipFile('orders.csv.zip')
zip_ref.extractall()
zip_ref.close()

4) Use panda library to extract and transform the dataset.
5) Using sqlalchemy to load the data to SQL-Server to a database.
6) Perform analysis by using SQL.
7) Establish a connection from the database to excel py using PowerQuery to create a report.
8) Create a report and save it as pdf file.

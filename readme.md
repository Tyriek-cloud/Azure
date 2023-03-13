# NYC DCA ETL

This was a project done in Azure Data Factory. 

I began by extracting data from New York City Open Data: https://opendata.cityofnewyork.us/

From there, I created a Blob Container within an existing storage account. Then I initialized Azure Data Factory to do a series of transformations on CSV files. I ultimately wanted to load data into a parquet file. The dataflow looks like this:

![image](https://user-images.githubusercontent.com/62261407/224825767-5fed9d29-175a-45cb-b914-6cea558afa56.png)

The final, loaded result of the ETL process resulted in the creation of a parquet file hosted in my container:

![image](https://user-images.githubusercontent.com/62261407/224824921-bf381f03-1c8f-4f73-bc84-ba38e659d3ab.png)

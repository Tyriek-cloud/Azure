# NYC DCA ETL

This was a project done in Azure Data Factory. 

I began by extracting data from New York City Open Data: https://opendata.cityofnewyork.us/

From there, I created a Blob Container within an existing storage account. Then I initialized Azure Data Factory to do a series of T-SQL transformations on CSV files. I ultimately wanted to load data into a parquet file. The dataflow looks like this:

![image](https://user-images.githubusercontent.com/62261407/224825767-5fed9d29-175a-45cb-b914-6cea558afa56.png)

The final, loaded result of the ETL process resulted in the creation of a parquet file hosted within a generated blob in the container:

![image](https://user-images.githubusercontent.com/62261407/224824921-bf381f03-1c8f-4f73-bc84-ba38e659d3ab.png)

I then went back into my container to look for any issues to trouble shoot. There were no issues to resolve, so I monitored activity in my container in a private dashboard:

![image](https://user-images.githubusercontent.com/62261407/225027680-e834c12a-e771-4284-bb86-89f2433afdbd.png)
![image](https://user-images.githubusercontent.com/62261407/225027790-1646533d-1a54-4b3c-abd2-552dfc35a519.png)
![image](https://user-images.githubusercontent.com/62261407/225027867-d180b4d3-7a78-4fb0-9275-c18ad4148b9e.png)

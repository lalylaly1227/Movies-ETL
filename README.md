# Movies-ETL

## Overview of the analysis
To create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. I will refactor the code from Module 8 to create one function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data—and performs the ETL process by adding the data to a PostgreSQL database.

<img width="354" alt="ETL" src="https://user-images.githubusercontent.com/105124485/177228704-70f32f19-6e77-4b75-bfd3-9e2048177408.png">

### Deliverable 1: Write an ETL Function to Read Three Data Files
I loaded the data from the different file types. Then I cleaned the data. 
<img width="820" alt="Del 1 Wiki to DataFrame" src="https://user-images.githubusercontent.com/105124485/177228267-d0af3695-86f7-429a-805d-2e31ae912efd.png">
<img width="819" alt="Del 1 Kaggle to DataFrame" src="https://user-images.githubusercontent.com/105124485/177228271-e4ca8641-05cb-443a-8080-d8a0225f7e8a.png">
<img width="362" alt="Del 1 MovieLens to DataFrame" src="https://user-images.githubusercontent.com/105124485/177228276-d78de90b-66fc-4080-88ba-207f12e4a9c2.png">


### Deliverable 2: Extract and Transform the Wikipedia Data
With the data from Deliverable 1 transform the Wikipedia data. Remove duplicates, rename files and rearrange the columns.
<img width="819" alt="Del 2 Wiki movies DataFrame" src="https://user-images.githubusercontent.com/105124485/177228287-002ae91b-cb0d-462a-b956-84f00a8670b8.png">
<img width="632" alt="Del 2 Wiki columns" src="https://user-images.githubusercontent.com/105124485/177228293-7a11615f-8d73-4a00-956f-a4c48b8b043d.png">


### Deliverable 3: Extract and Transform the Kaggle data
With the data from Deliverable 1 transform the Kaggle data. Remove duplicates, rename files and rearrange the columns
<img width="814" alt="Del 3 Wiki DataFrame" src="https://user-images.githubusercontent.com/105124485/177228299-5866dff5-8735-4786-b73c-e6443f700c4e.png">
<img width="815" alt="Del 3 Kaggle Metadata DataFrame" src="https://user-images.githubusercontent.com/105124485/177228304-6f738c36-52da-488f-af19-b6ceb3ff542f.png">
<img width="814" alt="Del 3 MovieLens DataFrame" src="https://user-images.githubusercontent.com/105124485/177228309-9e919665-3781-4c4a-8af3-5e54148ffaba.png">


#### Deliverable 4: Create the Movie Database
Using the files from the previous deliverable, create DataFrames and load the files to PostgreSQL, then read the data using pgAdmin and produce screenshots of the query results.
<img width="805" alt="Extraction progress" src="https://user-images.githubusercontent.com/105124485/177228323-e1e8a0fa-0c42-4fce-a070-c30c976c31f0.png">

<img width="82" alt="Del 4 movies_query" src="https://user-images.githubusercontent.com/105124485/177228328-63ff64aa-2bff-47c7-b27b-9db76330a751.png">
<img width="146" alt="Del 4 ratings_query" src="https://user-images.githubusercontent.com/105124485/177228337-07338fdb-bc15-49a0-97a2-ba44b342a5e8.png">


## Resources
### Data Sources: 
movies_metadata.csv file
	ratings.csv file
	Wikipedia-movies.json file		

### Software: 
Jupyter Notebooks, PostgreSQL, pgAdmin

## Results
I was able to clean up the data, remove unnecessary columns and join the files.  With the finished data, I was able to upload to the SQL server for further review.  

## Summary
There was a of 6,052 rows in the movie table and 26,024,289 rows in the ratings table.

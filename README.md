# nosql-challenge
---
## Part 1: Database and Jupyter Notebook Set Up 
### File: NoSQL_setup_starter.ipynb
* Importe the data provided in the establishments.json file from my Terminal. Named the database uk_food and the collection establishments. Copied the text you used to import your data from your Terminal to a markdown cell in your notebook.
* Imported the libraries needed: PyMongo and Pretty Print (pprint).
* Created an instance of the Mongo Client.
* Confirmed the database was created and data was properly loaded:
    * Listed the databases I have in MongoDB. Confirmed that uk_food is listed.
    * Listed the collection(s) in the database to ensure that establishments is there.
    * Found and displayed one document in the establishments collection using find_one and display with pprint.
* Assign the establishments collection to a variable to prepare the collection for use.
---
## Part 2: Update the Database
### File: NoSQL_setup_starter.ipynb
* Added the provided information on the new halal restaurant that just opened in Greenwich to the database.
*Found the BusinessTypeID for "Restaurant/Cafe/Canteen" and returned only the BusinessTypeID and BusinessType fields.
*Checked how many documents contain the Dover Local Authority. Then, removed any establishments within the Dover Local Authority from the database, and checked the number of documents to ensure they were deleted.
* Converted number values that were stored as strings.
    * Used "update_many" to convert "latitude" and "longitude" to decimal numbers.
    * Used "update_many" to convert "RatingValue" to integer numbers.
---
## Part 3: Exploratory Analysis
### File: NoSQL_analysis_starter.ipynb
* Found which establishments have a hygiene score equal to 20.
* Found establishments in London have a RatingValue greater than or equal to 4.
* Found the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours".
* Determined how many establishments in each Local Authority area have a hygiene score of 0.  Sorted the results from highest to lowest, and printed out the top ten local authority areas.
* The first 5 rows of my DataFrame results looked like following example.

![](Images\ExampleDataFrame_top5.png)
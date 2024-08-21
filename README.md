# nosql-challenge
The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. The editors of a food magazine, gave a task to the analysist and requested to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.

This challenge is devided into three parts:
Part:1 Database and Jupyter Notebook Set Up
Part:2 Update the Database
Part 3: Exploratory Analysis

Part:1 Database and Jupyter Notebook Set Up incldues: 
1. Import the data provided in the establishments.json file from your Terminal.
   Name the database uk_food and the collection establishments. Copy the text you used to import your data from your 
   Terminal to a markdown cell in your notebook. Import the data provided in the establishments.json file from your   
   Terminal. Name the database uk_food and the collection establishments. Within this markdown cell, copy the line of text 
   you used to import the data from your Terminal. This way, future analysts will be able to repeat your process.
   e.g.: Import the dataset with mongoimport
    --type json -d uk_food -c establishments --drop --jsonArray establishments.json

3. Within the notebook, import the libraries that are required: PyMongo and Pretty Print (pprint).
   

5. Create an instance of the Mongo Client.

6. Confirm that you created the database and loaded the data properly:

   4.1 List the databases you have in MongoDB. Confirm that uk_food is listed.
   4.2 List the collection(s) in the database to ensure that establishments is there.
   4.3 Find and display one document in the establishments collection using find_one and display with pprint.
7. Assign the establishments collection to a variable to prepare the collection for use.

Part 2: Update the Database inclues:

The magazine editors have some requested modifications for the database before performing any queries or analysis for them. They wants editor to use NoSQL_setup_starter.ipynb for this section they also wants to make the following changes to the establishments collection:

1. An exciting new halal restaurant just opened in Greenwich, but hasn't been rated yet. The magazine has asked you to 
   include it in your analysis.
2. Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.
3. Update the new restaurant with the BusinessTypeID you found.
4. The magazine is not interested in any establishments in Dover, so check how many documents contain the Dover Local 
   Authority. Then, remove any establishments within the Dover Local Authority from the database, and check the number of 
   documents to ensure they were deleted.
5. Some of the number values are stored as strings, when they should be stored as numbers.
   5.1 Use update_many to convert latitude and longitude to decimal numbers.
   5.2 Use update_many to convert RatingValue to integer numbers.

Part 3: Exploratory Analysis

1. RatingValue refers to the overall rating decided by the Food Authority and ranges from 1-5. The higher the value, the 
    better the rating.Note: This field also includes non-numeric values such as 'Pass', where 'Pass' means that the 
    establishment passed their inspection but isn't given a number rating. We will coerce non-numeric values to nulls during 
    the database setup before converting ratings to integers.
2. The scores for Hygiene, Structural, and ConfidenceInManagement work in reverse. This means, the higher the value, the 
    worse the establishment is in these areas.
3. Use the following questions to explore the database, and find the answers, so you can provide them to the magazine 
   editors.Unless otherwise stated, for each question: Use count_documents to display the number of documents contained in 
   the result.
4. Display the first document in the results using pprint.
5. Convert the result to a Pandas DataFrame, print the number of rows in the DataFrame, and display the first 10 rows.
   5.1 Which establishments have a hygiene score equal to 20?
   5.2 Which establishments in London have a RatingValue greater than or equal to 4?
   5.3 What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new 
       restaurant added, "Penang Flavours"?

Refernce: 1. BCS Classroom activites and codes
          2. Used Xpert Learning Assistant 
          3. Took help of classmates
          4. use onlien resources and ChatGpt



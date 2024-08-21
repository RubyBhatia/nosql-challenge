# nosql-challenge
The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. The editors of a food magazine, gave a task to the analysist and requested to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.

This challenge is devided into two parts:
Part:1 Database and Jupyter Notebook Set Up
Part:2 Part 2: Update the Database

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

   

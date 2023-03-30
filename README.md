# nosql-challenge

The purpose of this challenge is to evaluate some of the ratings data given by The UK Food Standards Agency in order to help journalists at 'Eat Safe, Love' decide where to focus future articles.

## Database and Jupyter Notebook Set up

Using NoSQL_setup_starter.ipynb for this section, import the data provided in the establishments.json file from Terminal. Name the database uk_food and the collection establishments. Copy the text used to import your data from Terminal to a markdown cell in the notebook.

## Update the Database

Using NoSQL_setup_starter.ipynb for this section, update the establishments collection to add the new "Penang Flavours" restaurant and update its BusinessTypeID by finding the BusinessTypeIDs for other "Restaurant/Cafe/Canteen" businesses.
Remove any establishments within the Dover Local Authority.
Update the latitude and longitude of the restaurant to decimal numbers.

## Exploratory Analysis

Using NoSQL_analysis_starter.ipynb for this section.
Be aware that RatingValue refers to the overall rating decided by the Food Authority and ranges from 1-5. The higher the value, the better the rating. Note: This field also includes non-numeric values such as 'Pass', where 'Pass' means that the establishment passed their inspection but isn't given a number rating.
The scores for Hygiene, Structural, and ConfidenceInManagement work in reverse. This means, the higher the value, the worse the establishment is in these areas.
Questions the magazine journalists want answered:
1. Which establishments have a hygiene score equal to 20?
2. Which establishments in London have a RatingValue greater than or equal to 4?
3. What are the top 5 establishments with a RatingValue of '5', sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"? Note: You will need to compare the geocode to find the nearest locations. Search within 0.01 degree on either side of the latitude and longitude.
4. How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.

Note of Source Code: Beyond the starter code and using class examples to guide my work, I had the online Learning Assistant help with the syntax of my establishments.update_one code when updating the BusinessTypeID of the new restaurant in the NoSQL_setup_starter.ipynb notebook, and my TA helped me with the query line setup when finding the top 5 establishments with RatingValues of 5 sorted by lowest hygiene score that were closest to the new restaurant added in the NoSQL_analysis_starter.ipynb notebook.

# NoSQL Challenge: UK Food Establishments Analysis

## Project Overview
This project analyzes food hygiene ratings data sourced from the UK Food Standards Agency. The task involves importing JSON data into a MongoDB database, performing several update operations (such as inserting new data, updating records, and deleting unwanted documents), and running exploratory queries using Jupyter notebooks. The overall analysis supports investigative questions for a food magazine, "Eat Safe, Love," such as assessing hygiene scores, filtering establishments in London, and comparing nearby high-rating establishments to the newly added "Penang Flavours" restaurant.

## Files and Directories

- **Resources/establishments.json**  
  A JSON file containing the establishments data used to create the MongoDB database.

- **NoSQL_setup_starter.ipynb**  
  This Jupyter Notebook covers:
  - Importing the JSON data into the MongoDB database (`uk_food`) under the `establishments` collection.
  - Verifying database and collection creation.
  - Inserting and updating a new restaurant ("Penang Flavours").
  - Deleting documents from the Dover Local Authority.
  - Updating data types, converting coordinate and rating values from strings to their proper numeric types.

- **NoSQL_analysis_starter.ipynb**  
  This Jupyter Notebook performs the exploratory analysis queries:
  - Querying establishments with a hygiene score of 20.
  - Filtering establishments in London with a `RatingValue` greater than or equal to 4 (using a `$regex` for broader matching).
  - Finding the top 5 establishments with a `RatingValue` of 5, sorted by the lowest hygiene score and near the "Penang Flavours" restaurant.
  - Aggregating establishment counts by local authority where the hygiene score is 0, and sorting these counts in descending order.

## Disclaimer
**Disclaimer:**  
*Code is my own, I used MS Copilot/Github Copilot in some instances where I got stuck or had questions to move forward. I did some standard online research as well to better understand some of the code structure I was making.*


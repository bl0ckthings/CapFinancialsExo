# Steps to solve this exercise

I first setup the environment and started to analyze the codebase starting from the backend side.

Once i understood how the code worked, I created a new type for the second source file and changed the company type structure to match requirements. I also created a new collections for the new file.

In order to populate my MongoDB DB, I copied the ingest-source1 script file and adapted it to work for source2. Once done I was able to run the script and see the database fufilled with my new values and merged the data needed from source2 into companies collection.
At that stage, I started the frontend and could see the values with the new fields, i made sure to add the new fields and retrieve new values.

Then, i needed to add the features asked in the assignment starting by the filter by website using mongoDb $nin query predicate operator and filter by numberOfEmployees using the existing helper function 'addRange'.

Finally, I worked on the front end to add new numberOfEmployees and Website filter.

PS : I added a new feature that allows to load data from backend when the Vue page loads up using watch and onMounted from Vue library.


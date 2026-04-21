# Steps to solve this exercise

1. Initial Setup & Codebase Analysis

I started by setting up the environment and analyzing the backend codebase to understand how the existing system works and how data flows through it.

2. Backend Changes
New Source Integration
Created a new type for the second source file.
Updated the company type structure to match the new requirements.
Added a new collection dedicated to the second source.
Data Ingestion
Duplicated the existing ingest-source1 script.
Adapted it to support the second source (source2).
Ran the script to populate the MongoDB database.

At this point:

The database was successfully filled with data from both sources.
Relevant fields from source2 were merged into the companies collection.
3. Frontend Verification
Started the frontend application.
Confirmed that the new fields were properly displayed.
Updated components to include and retrieve the new data fields.
4. Feature Implementation
Filtering Features
Filter by website
Implemented using MongoDB’s $nin query operator.
Filter by number of employees
Implemented using the existing helper function addRange.
5. Frontend Enhancements
Added UI elements for:
numberOfEmployees filter
website filter
Ensured these filters correctly interact with backend queries.
6. Additional Improvement
Implemented automatic data loading on page initialization using Vue’s onMounted() hook.
This ensures data is fetched from the backend as soon as the page loads.

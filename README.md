# Project Implementation Overview

## 1. Initial Setup & Codebase Analysis

I first setup the environment and started to analyze the codebase starting from the backend side.

Once I understood how the code worked, I moved on to implementing the required changes.

---

## 2. Backend Changes

### New Source Integration

- Created a new type for the second source file.
- Changed the `company` type structure to match the requirements.
- Created a new collection for the second source.

### Data Ingestion

In order to populate my MongoDB database:

- Copied the `ingest-source1` script.
- Adapted it to work for `source2`.
- Executed the script to insert data.

After this step:
- The database was filled with the new values.
- Data from `source2` was merged into the `companies` collection.

---

## 3. Frontend Integration

- Started the frontend application.
- Verified that the new fields were correctly displayed.
- Updated the frontend to retrieve and display the new values.

---

## 4. Feature Implementation

### Filter by Website

- Implemented using MongoDB `$nin` query predicate operator.

### Filter by Number of Employees

- Implemented using the existing helper function `addRange`.

---

## 5. Frontend Enhancements

- Added filters in the UI for:
  - `numberOfEmployees`
  - `website`
- Ensured proper communication with backend filtering logic.

---

## 6. Additional Feature

- Added automatic data loading when the Vue page loads.
- Implemented using `onMounted()` from the Vue library.

---

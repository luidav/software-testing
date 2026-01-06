# Goodreads – Manual Test Cases

This document contains a curated selection of manual test cases designed to validate the search functionality of the Goodreads web application.
The full test suite is maintained in Google Sheets; this file highlights representative examples used for portfolio purposes.

---

## TC-001 – Search Book by Exact Title

**Feature:** Search  
**Priority:** High  

### Preconditions
- User is on the Goodreads homepage.

### Steps
1. Locate the search bar.
2. Enter a full and valid book title (e.g., "Atomic Habits").
3. Submit the search.

### Expected Result
A results page is displayed showing books that exactly match the entered title, ranked by relevance.

---

## TC-002 – Search Book by Partial Title

**Feature:** Search  
**Priority:** Medium  

### Preconditions
- User is on the Goodreads homepage.

### Steps
1. Locate the search bar.
2. Enter a partial book title (e.g., "Hobb").
3. Submit the search.

### Expected Result
The system returns relevant results matching the partial input (e.g., "The Hobbit").

---

## TC-003 – Search Book by Author Name

**Feature:** Search  
**Priority:** High  

### Preconditions
- User is on the Goodreads homepage.

### Steps
1. Locate the search bar.
2. Enter a valid author name (e.g., "J.K. Rowling").
3. Submit the search.

### Expected Result
Books written by the specified author are displayed in the results page.


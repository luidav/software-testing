# Software Testing Project - Goodreads

Goodreads is a popular platform among book lovers worldwide. As a frequent user, I decided to look at this tool from a different perspective: that of a software tester. This project summarizes a manual testing process I carried out on key features of the site, applying logical thinking, structured exploration, and clear technical documentation.

---

`## Project Objective`

To demonstrate my ability to apply manual testing in a real-world application, using a professional approach. This project includes test cases, exploratory testing, bug documentation, and technical insights.

---

## Features Tested

- User sign up and sign in
- Redirection to other pages in the sign in page
- Book search
- Author search
- Group search
- Quote search
- List search
- People search
- Adding books to the "Want to Read" list  
- Rating and reviewing books

---

## Testing Approaches Used

- **Positive testing** – Validating expected flows  
- **Negative testing** – Simulating invalid inputs and errors  
- **Exploratory testing** – Free navigation to detect unexpected behaviors  
- **Usability observations** – Suggestions to improve user experience

---

## Test Scenarios

### Test Escenario 1: User Login – Valid Credentials
**Feature:** Login

**Scenario:** User logs in using a valid email and password

**Steps:**

1. Navigate to Goodreads homepage

2. Click on the “Sign In” button

3. Enter a registered email and correct password

4. Click “Sign In”

- **Expected Result:** User is redirected to their homepage
- **Actual Result:** ✅ As expected
- **Status:** Passed


### Test Escenario 2: Search for a Book – Valid Input 
**Feature:** Book Search

**Scenario:** Search using a valid book title

**Steps:**

1. Go to the Goodreads homepage

2. Locate the search bar

3. Type the title “Atomic Habits”

4. Press Enter or click the search icon

- **Expected Result:** A list of books matching “Atomic Habits” appears
- **Actual Result:** ✅ As expected
- **Status:** Passed


In the next link you can find more basic test scenarios for Goodreads:

[ https://docs.google.com/spreadsheets/d/1W_JuKU7X42Rel6V1detaIfPSsZus5T1Y0k6cJTkmsPQ/edit?usp=sharing ].

---

## Test Cases

### Test Case 1: Search a book by partial title
**Priority:** Medium

**Feature:** Book search

**Scenario:** User searches for a book using only part of the title

**Steps:**

1. Navigate to the Goodreads homepage.

2. Locate the search bar.

3. Type a partial title, for example: Hobb (for The Hobbit).

4. Press Enter or click the search icon.

-**Expected Result:** Search suggestions appear, including the full title (e.g., The Hobbit), or the results page shows relevant books matching the input.
- **Actual Result:** ✅ As expected.
- **Status:** Passed.


### Test Case 2: Search a book by author name
**Feature:** Book Search

**Scenario:** User searches for books by entering an author's name

**Steps:**

1. Navigate to the Goodreads homepage.

2. Locate the search bar.

3. Type the author’s name (e.g., “J.K. Rowling”).

4. Press Enter or click the search icon.

**Expected Result:** The results page displays books written by the author, ranked by popularity or relevance.

**Priority:** High

In the next link you can find more test cases for Goodreads:

[ https://docs.google.com/spreadsheets/d/1nJAofkbqEoeYHENtsDXXdKLm6iz6WKpXrVGRfb1A2-k/edit?usp=sharing ].

---

## Bugs Found

### Bug 1: Email Field Accepts Invalid or Misspelled Domains

**Section:** Sign Up / Sign In  
- **Severity:** Medium  
- **Summary:** The system accepts email addresses with invalid or misspelled domains (e.g., `abc@gmal.com`) without displaying any warning.  
- **Expected Result:**  
  The sign-up process should prevent submission and display a validation message informing the user that the email may be invalid.  
- **Actual Result:**  
  Account creation proceeds successfully even when the domain contains obvious typos.  
- **Impact:**  
  May lead to undelivered confirmation or notification emails and reduce data quality.

---

### Bug 2: Search Fails to Handle Misspelled Book Titles
- **Section:** Search Functionality  
- **Severity:** Medium  
- **Summary:** The search bar does not recognize or correct common misspellings of book titles.  
- **Steps to Reproduce:**  
  1. Enter a misspelled title such as “Hary Poter”.  
  2. Press Enter or click the search icon.  
- **Expected Result:**  
  The system should propose suggestions such as “Did you mean: *Harry Potter*?” or return fuzzy-matched relevant items.  
- **Actual Result:**  
  No suggestions or relevant results are returned.  
- **Impact:**  
  Leads to poor search experience and makes relevant content harder to discover.
[https://docs.google.com/spreadsheets/d/1Eiseva5nc-eWWw8Aesd8KT1BzJ4TVaVsRAlC0BxeM4g/edit?usp=sharing]
---


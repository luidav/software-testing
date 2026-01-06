# Goodreads – Defect Reports

This document contains defects identified during manual testing of the Goodreads web application.
The bugs were found while testing core user flows such as authentication and search functionality.

---

## BUG-001 – Name and Last Name Field: Validation Inconsistency

**Section:** Sign Up / Sign In  
**Severity:** Low  
**Priority:** Low  

### Steps to Reproduce
1. Navigate to Home page.
2. Click "Sign Up with email".
3. In the "Your name" field, enter text containing numbers or special characters (e.g., John123, Doe@!).
4. Complete the remaining fields.
5. Click "Create account" button.

### Expected Result
The "Your name" field should accept only alphabetic characters (and optionally spaces or accented letters). If invalid characters are entered, the system should display a validation message such as: "Please enter a valid name (letters only)".

Alternatively, if the field is meant to act as a username, the label could be adjusted to clarify its purpose, e.g., "Display name" or "Username".

### Actual Result
The form successfully creates an account even when the "Your name" field contains numbers or special characters.

### Impact
This may lead to user confusion regarding the intended use of the field and potential data quality issues if the system expects structured name data for personalization, communication, or reporting purposes.

---

## BUG-002 – Email Field Accepts Invalid or Misspelled Domains

**Section:** Sign Up / Sign In  
**Severity:** Medium  
**Priority:** Medium  

### Steps to Reproduce
1. Navigate to the Sign Up page.
2. Enter an email with a misspelled domain (e.g., abc@gmal.com).
3. Complete the remaining required fields.
4. Submit the form.

### Expected Result
The system should prevent account creation and display a validation message indicating the email domain may be invalid.

### Actual Result
The account is created successfully without any warning.

### Impact
This may lead to undelivered emails and poor data quality.

---

## BUG-003 – Search Does Not Handle Misspelled Book Titles

**Section:** Search  
**Severity:** Medium  
**Priority:** Medium  

### Steps to Reproduce
1. Locate the search bar.
2. Enter a misspelled book title (e.g., "Hary Poter").
3. Submit the search.

### Expected Result
The system should suggest a corrected title (e.g., "Did you mean: Harry Potter?") or return relevant results.

### Actual Result
No suggestions or relevant results are displayed.

### Impact
This negatively affects search usability and content discoverability.


**Full defect log:**
[View complete defect report](https://docs.google.com/spreadsheets/d/1Eiseva5nc-eWWw8Aesd8KT1BzJ4TVaVsRAlC0BxeM4g/edit?usp=sharing).

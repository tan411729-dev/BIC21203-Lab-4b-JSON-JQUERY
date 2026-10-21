# BIC21203 Web Development — Lab 4b: Client-Side Scripting (JSON and jQuery)

## Student Information
- **Name:** Tan Boon Hong
- **Matric No:** AI250264
- **Course:** BIC21203 Web Development
- **Section:** 8

---

## Overview
This laboratory exercise covers practical client-side data handling and library integration, including creating structured JSON datasets, fetching and parsing JSON data asynchronously via the native JavaScript `fetch()` API with error handling, and comparing native DOM manipulation with jQuery (v4.0.0).

---

## Setup & Instructions to Run
1. Clone or download this repository to your local machine.
2. Ensure you have a local web server running (e.g., **XAMPP Apache** or **VS Code Live Server**).
> *Note: Question 2 uses the `fetch()` API and must not be run directly via `file://` due to browser CORS policies.*
3. Place the project folder in your local web server root directory (e.g., `xampp/htdocs/`).
4. Access the files through your browser:
   - `http://localhost/.../books.html`
   - `http://localhost/.../jquery-dom.html`

---

## Tasks & Output Screenshots

### Question 1: Create and Structure JSON Data
- **Description:** Created a valid `books.json` dataset featuring a top-level `books` array containing two book objects with typed properties (`title`, `author`, `publicationYear`, and a `genres` array of strings).
- **Validation:** Confirmed valid JSON structure via JSONLint / JSON Validator.
- **Output:**
  ![Question 1 Output - JSON Code](screenshots/Q1%20json.png)
  ![Question 1 Output - JSON Validation](screenshots/Q1%20validate.png)

---

### Question 2: Retrieve and Display JSON Data
- **Description:** Uses the native `fetch()` API to asynchronously retrieve `books.json` and safely renders the first book's title, the second book's author, and both books' genres grouped by title. Includes error handling for failed requests.
- **Output:**
  ![Question 2 Error Handling](screenshots/Q2%20failure.png)
  ![Question 2 Success Output](screenshots/Q2%20success.png)

---

### Question 3: Compare Native JavaScript and jQuery
- **Description:** Implements DOM text replacement using `.text()`, applies CSS styling using `.addClass()`, and registers click event listeners using `.on("click", ...)` via jQuery 4.0.0 CDN.
- **Output:**
  ![Question 3 Output - Style and Text](screenshots/Q3%20before.png)
  ![Question 3 Output - Alert](screenshots/Q3%20after.png)

## Conceptual Comparison
- **Advantage of Native JavaScript:**
  Native JavaScript is faster to load and does not require external libraries.
- **Situation where projects still use jQuery:**
  Projects use jQuery to maintain legacy code or support existing jQuery plugins.

# Awesome Kartikey Form Validator

A simple, clean, and effective client-side form validator built with vanilla HTML, CSS, and JavaScript. This project demonstrates fundamental form validation techniques using HTML5 constraint validation and JavaScript for enhanced user feedback.

## Description

This project provides a basic sign-up form with client-side validation for common fields like name, phone number, email address, website URL, and password confirmation. It leverages built-in HTML5 validation attributes and complements them with JavaScript to provide real-time feedback to the user, including visual cues and messages.

## Features

- **HTML5 Validation:** Utilizes `required`, `minlength`, `maxlength`, `pattern`, `type="email"`, and `type="url"` attributes for basic validation.
- **JavaScript Enhancements:**
  - Checks if password and confirm password fields match.
  - Provides clear success or error messages to the user.
  - Changes input border colors based on validity (`:valid`/`:invalid` CSS pseudo-classes and JS for password match).
- **Real-time Feedback:** Visual cues (border colors) update as the user interacts with the form (though full real-time feedback per input requires more JS). Overall validation occurs on submit.
- **Clean UI:** Simple and focused user interface styled with CSS.
- **Lightweight:** No external libraries or frameworks required (besides Google Fonts).

## Tech Stack

- **HTML5:** For structure and semantic form elements, including built-in validation attributes.
- **CSS3:** For styling, layout (Flexbox), and visual feedback (e.g., `:valid`, `:invalid` pseudo-classes).
- **Vanilla JavaScript:** For handling form submission, custom validation logic (password matching), DOM manipulation, and displaying feedback messages.

## Setup Instructions

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/awesome-kartikey/form-validator.git
    ```
2.  **Navigate to the directory:**
    ```bash
    cd form-validator
    ```
3.  **Open `index.html`:**
    Simply open the `index.html` file in your web browser. No build steps or local server is strictly required for basic functionality, although running it via a simple live server extension in your code editor is recommended for development.

## Usage

1.  Open the `index.html` file in your browser.
2.  Fill out the sign-up form fields.
3.  Observe the input border colors change based on HTML5 validation rules (green for valid, red for invalid).
4.  Ensure the "Password" and "Confirm Password" fields match.
5.  Click the "Register" button.
6.  A message will appear below the form indicating whether the registration was successful (all fields valid and passwords match) or if there are errors.
7.  If successful, the form data is logged to the browser's developer console (Note: data is not actually sent to a server in this version).

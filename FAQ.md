# Frequently Asked Questions (FAQ)

### Q1: What is the main purpose of this project?

**A:** This project serves as a simple demonstration of client-side form validation techniques using standard web technologies: HTML5, CSS3, and Vanilla JavaScript. It shows how to validate various input types and provide feedback to the user without relying on external libraries.

### Q2: How does the validation work?

**A:** Validation uses a combination of:

1.  **HTML5 Constraint Validation API:** Attributes like `required`, `pattern`, `minlength`, `maxlength`, and input `type` (like `email`, `url`) allow the browser to perform basic checks automatically. The `form.checkValidity()` method in JavaScript leverages this API.
2.  **CSS Pseudo-classes:** `:valid` and `:invalid` CSS pseudo-classes are used to style input fields based on their HTML5 validation state (e.g., changing border colors).
3.  **JavaScript:** Custom JavaScript logic (`script.js`) is used to:
    - Trigger validation on form submission.
    - Specifically compare the "Password" and "Confirm Password" fields, as this cannot be done with HTML5 attributes alone.
    - Update a message area (`#message`) to display overall success or error information.
    - Dynamically change border colors for password fields based on the match status.

### Q3: Is the form data actually submitted or saved anywhere?

**A:** No. In its current state, the project only performs _client-side_ validation. When the form is successfully validated, the `storeFormData` function in `script.js` merely collects the form data into a JavaScript object and logs it to the browser's developer console using `console.log(user)`. There is no backend or database interaction.

### Q4: Can I customize the validation rules or appearance?

**A:** Yes.

- **Validation Rules:** You can modify the HTML attributes (`pattern`, `minlength`, etc.) in `index.html` or add more complex validation logic in `script.js`.
- **Appearance:** You can change the styles (colors, layout, fonts) by editing the `style.css` file.

### Q5: What browsers are supported?

**A:** The project uses features widely supported in modern web browsers (HTML5 forms, CSS3, basic DOM manipulation, `checkValidity`). It should work correctly on recent versions of Chrome, Firefox, Safari, Edge, and other modern browsers. Issues might occur on very old browsers like Internet Explorer that lack full support for these features.

### Q6: Does this project have any external dependencies?

**A:** The only external resource used is Google Fonts (`Sen` font) loaded via the `@import` rule in `style.css`. The core functionality relies solely on standard browser APIs (HTML, CSS, JS).

### Q7: Is this validation secure?

**A:** No. Client-side validation is essential for good user experience (UX) as it provides immediate feedback. However, it is **not secure** on its own because users can bypass it (e.g., by disabling JavaScript or manipulating the requests). **Always implement comprehensive server-side validation** to ensure data integrity and security. This project focuses only on the client-side aspect.

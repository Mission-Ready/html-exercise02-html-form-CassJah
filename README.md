# 02 Exercise - HTML Forms

## Brief

Build a _Create an account_ form with various input types in HTML

![form stacked](docs/form-stacked.png)

---

## Rationale

Almost every web app will use forms in one incarnation or another, so HTML forms will be an important part of your skillset.

---

## Getting Started

1. `git clone` this repository into your main exercise folder.
- If you are not too sure how to do it, please follow this [video](https://www.loom.com/share/8a0d420720a94cb18021c2f418b19ae8?sid=f960095f-5b12-4428-a628-441689aec48e)
 to see how to git clone the repository into your device.
2. The code for this exercise should go into the `/Submission` folder.

---

## Exercise Part A - Add Form Elements

1. Create an `index.html` file in the `Submission` folder. Create the HTML base code by typing `!` and pushing `tab`
2. Add a heading inside the body: `<h1>Create an account</h1>` inside the `<body>` element.
3. Create a `<form></form>` element after the `<h1>`
4. Add an `action` and `method` attribute to your form, so it looks like the below snippet:

   ```html
   <form action="mailto:phoebes@missionreadyhq.com" method="post"></form>
   ```

   This will make your form submission be emailed to your instructor.

5. Inside your `<form>` element, add the following HTML form elements, with the corresponding labels and input types.

   - Ensure each of your labels is linked to your input by using the `for` attribute, that matches the `id` of the form input
   - Ensure each of your inputs has the `name` attribute.

     ```html
     <label for="name">Name</label> <input id="name" name="name" type="text" />
     ```

   | Label                  | Input name | Input type | Options                |
   | ---------------------- | ---------- | ---------- | ---------------------- |
   | Name                   | name       | text       | n/a                    |
   | Email                  | email      | email      | n/a                    |
   | Password               | password   | password   | n/a                    |
   | Address                | address    | textarea   | n/a                    |
   | Country                | country    | select     | New Zealand, Australia |
   | Sign up to newsletter? | newsletter | checkbox   | n/a                    |

6. Add a submit button before the closing `</form>` tag:

   ```html
   <button type="submit">Create account</button>`
   ```

7. Test your page in your web browser

   - Do your form inputs look correct? For example, does it hide the text when you type your password? Do your checkbox and select work correctly?
   - When you click the label, does it automatically highlight the form input?

     ![label highlight](docs/label-highlight.gif)

8. Fill in the form fields and submit the form. All things going well, you should get a success message. If you get an error message, try and fix the error.

9. You will notice all the form elements are on the same line. This is because form elements are `inline` by default.

   ![inline form](docs/form-inline.png)

   To make everything appear in its own line, wrap each label/input combination in a `<div>` element. For example:

   ```html
   <div>
     <label for="name">Name</label>
     <input id="name" name="name" type="text" />
   </div>
   ```

10. Ensure your HTML is valid using the [W3C HTML Validator](https://validator.w3.org/#validate_by_input).
11. Commit your code to git

Your form should look like the screenshot below. It's not well designed, but it's functional.

![form stacked](docs/form-stacked.png)

**Acceptance criteria**

- All form fields are present that are listed in the specification
- When clicking a label, it focuses on the corresponding form input
- When a user pushes enter while in a form element, the form submits
- When the form submits, it displays the Formspree confirmation page
- The form inputs have appropriate names, so when the form is submitted the correct data appears in the Formspree email

## Exercise Part B - Make name and email required inputs

It's possible to make form inputs required, by using the `required` attribute. You can read more about [The required attribute on MDN](https://developer.mozilla.org/en-US/docs/Learn/Forms/Form_validation#The_required_attribute)

1. Make the _Name_ and _Email_ form inputs required, by adding the `required` attribute to the inputs.

   ```html
   <input id="name" name="name" type="text" required />
   ```

2. Commit your code to git

**Acceptance criteria**

- If the name input is empty, the form can not be submitted
- If the email input is empty, the form can not be submitted

## Exercise Part C - Add a reset button

We can also have a button for reset all the input.

1. Now try to create one `reset` button.

   ```html
   <input type="reset" value="Reset" />
   ```

2. Your button section should look like
   ![Alt text](docs/image.png)

**Acceptance criteria**

- When you click Reset button, all the input field should become empty without any text inside.

---

# Submit your Exercise

- [ ] Push your code with your folder back to this Github Repository
- [Tutorial Video for push your code](https://www.loom.com/share/e6fb52378eaf4636b62fc302f15b5aeb?sid=e6f68797-9dab-42b5-ae76-745316994fa6)

# Walkthrough Solution Videos

- [Video](https://www.loom.com/share/e51c73c9da5540789a7d0468b4b6fd14)

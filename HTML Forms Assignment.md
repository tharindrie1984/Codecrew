# HTML Forms Assignment – Student Registration Portal

Create a complete HTML form for a **School Student Registration Portal** using only HTML form tags and attributes.
The goal of this assignment is to practice creating structured forms, collecting different types of user input, and using HTML form attributes correctly.

---

# Assignment Overview

Imagine your school is launching an online portal where students can register for clubs, competitions, and events. Your task is to design the registration page using HTML forms only.

⚠️ **No CSS and No JavaScript** are allowed.

You must use proper HTML form elements and attributes to make the form meaningful and user-friendly.

---

# Learning Objectives

By completing this assignment, students will learn to:

* ✓ Create HTML forms using the `<form>` tag
* ✓ Use different input types correctly
* ✓ Apply important form attributes
* ✓ Organize form elements clearly
* ✓ Use labels for accessibility
* ✓ Create dropdowns, radio buttons, and checkboxes
* ✓ Understand form validation basics

---

# Required HTML Tags

Your assignment must include the following tags:

| Tag          | Purpose                  |
| ------------ | ------------------------ |
| `<form>`     | Create the form          |
| `<input>`    | User input               |
| `<label>`    | Label form fields        |
| `<textarea>` | Multi-line text          |
| `<select>`   | Dropdown list            |
| `<option>`   | Dropdown choices         |
| `<button>`   | Submit/reset buttons     |
| `<fieldset>` | Group related data       |
| `<legend>`   | Title for grouped fields |

---

# Required Input Types

You must use all of these input types at least once:

* `text`
* `password`
* `email`
* `number`
* `date`
* `radio`
* `checkbox`
* `file`
* `tel`
* `submit`
* `reset`

---

# Required Attributes

Your form must correctly use these attributes:

| Attribute     | Purpose                 |
| ------------- | ----------------------- |
| `placeholder` | Display hint text       |
| `required`    | Mandatory field         |
| `value`       | Default value           |
| `readonly`    | Read-only field         |
| `disabled`    | Disabled field          |
| `maxlength`   | Limit text length       |
| `min` / `max` | Limit numbers           |
| `checked`     | Default checked option  |
| `selected`    | Default dropdown option |
| `name`        | Identify form data      |
| `id`          | Connect labels          |
| `for`         | Link label to input     |

---

# Assignment Requirements

## Section 1 – Student Information

Create a fieldset titled **"Student Information"** containing:

1. Full Name
2. Admission Number
3. Email Address
4. Telephone Number
5. Date of Birth
6. Password

### Requirements

* Full Name must have:

  * `placeholder`
  * `maxlength="30"`
  * `required`

* Admission Number:

  * Must be `readonly`
  * Value should already appear

* Email:

  * Must use `type="email"`

* Telephone:

  * Must use `type="tel"`

* Password:

  * Must use `type="password"`

---

# Section 2 – Academic Details

Create another fieldset titled **"Academic Details"**.

Include:

1. Grade Selection
2. Stream Selection

---

## Grade Selection

Use a dropdown list (`<select>`).

Options:

* Grade 6
* Grade 7
* Grade 8
* Grade 9
* Grade 10
* Grade 11
* Grade 12
* Grade 13

Requirements:

* One option must be selected by default.

---

## Stream Selection

Use radio buttons for:

* Science
* Commerce
* Arts
* Technology

Requirements:

* Only one option can be selected at a time.
* One option must already be checked.

---

# Section 3 – Club Registration

Create a fieldset titled **"Club Registration"**.

Use checkboxes for the following clubs:

* ICT Club
* AI Club
* Media Unit
* Chess Club
* Robotics Club

Requirements:

* Students should be able to select multiple clubs.
* At least one checkbox should already be checked.

---

# Section 4 – Additional Details

Include:

1. Upload Student Photo
2. Short Description About Yourself

---

## Upload Student Photo

* Use `type="file"`

---

## About Yourself

* Use `<textarea>`
* Minimum 4 lines
* Add placeholder text

---

# Section 5 – Terms and Conditions

Add:

* A checkbox saying:

  `"I agree to the school rules and regulations"`

Requirements:

* Must be required before submission.

---

# Section 6 – Buttons

Add:

1. Submit Button
2. Reset Button

---

# Page Structure Rules

Your page must:

* Use proper heading hierarchy
* Use `<fieldset>` and `<legend>` correctly
* Use labels for every form control
* Keep related fields grouped together
* Use meaningful attribute values

---

# Sample Skeleton

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Registration Form</title>
</head>

<body>

<h1>School Student Registration Portal</h1>

<form>

    <fieldset>
        <legend>Student Information</legend>

        <!-- Add form controls here -->

    </fieldset>

    <fieldset>
        <legend>Academic Details</legend>

        <!-- Add form controls here -->

    </fieldset>

    <fieldset>
        <legend>Club Registration</legend>

        <!-- Add form controls here -->

    </fieldset>

    <fieldset>
        <legend>Additional Details</legend>

        <!-- Add form controls here -->

    </fieldset>

    <button type="submit">Submit</button>
    <button type="reset">Reset</button>

</form>

</body>
</html>
```

---

# Common Mistakes to Avoid

❌ Different `name` values for radio buttons

```html
<input type="radio" name="science">
<input type="radio" name="commerce">
```

✅ Correct

```html
<input type="radio" name="stream">
<input type="radio" name="stream">
```

---

❌ Missing labels

```html
<input type="text">
```

✅ Correct

```html
<label for="fname">Full Name</label>
<input type="text" id="fname">
```

---

❌ Forgetting the `required` attribute

```html
<input type="email">
```

✅ Correct

```html
<input type="email" required>
```

---

# Bonus Challenge 🏆

For an extra 10 marks:

* ⭐ Use the `<datalist>` tag
* ⭐ Add hidden input fields
* ⭐ Use `autocomplete` attribute
* ⭐ Add pattern validation for telephone number
* ⭐ Use `<optgroup>` inside dropdowns

---

# Submission Guidelines

1. Save the file as:

```text
registration_form.html
```

2. Add a comment block at the top including:

   * Name
   * Class
   * Index Number

3. Open the page in a browser and test:

   * Radio button behavior
   * Required field validation
   * Submit and reset buttons

---

# Marking Scheme

| Criteria                   | Marks |
| -------------------------- | ----- |
| Correct Form Structure     | 20    |
| Proper Use of Input Types  | 20    |
| Correct Use of Attributes  | 20    |
| Labels and Accessibility   | 15    |
| Fieldsets and Organization | 15    |
| Validation Features        | 10    |

**Total = 100 Marks**

Good Luck 🚀

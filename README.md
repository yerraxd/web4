# Forms Assignment

A small multi-page website that demonstrates HTML forms, built-in browser validation and Bootstrap 5 validation styles.

## Project structure

```
.
├── index.html    # Task 0. Contact Form
├── task2.html    # Task 2. Bootstrap Validation Styles
├── task3.html    # Task 3. Registration Form
├── style.css     # Custom styles (form container, small tweaks)
└── README.md
```

## Technologies

- HTML5 (form elements and validation attributes)
- CSS3 (`style.css`)
- Bootstrap 5.3.3 (via CDN: CSS and JS bundle)

No custom JavaScript is used. Only the Bootstrap bundle is loaded, and it is needed for the collapsible navbar.

## Pages

### Task 0. Contact Form (`index.html`)

A basic contact form with plain HTML validation.

- **Name**: required, 3 to 20 characters
- **Email**: required, must be a valid email (`type="email"`)
- **Message**: textarea
- **Submit** button

### Task 2. Bootstrap Validation Styles (`task2.html`)

A contact form styled with Bootstrap form classes and validation feedback.

- Two-column layout for Name and Email (`row`, `col-md-6`)
- Required fields: Name (3 to 20 characters), Email, Message
- `valid-feedback` and `invalid-feedback` messages under each field
- **Submit** and **Reset** buttons

### Task 3. Registration Form (`task3.html`)

A full registration form with different input types.

| Field | Type | Validation |
|---|---|---|
| First Name | text | required, 2 to 30 characters |
| Last Name | text | required, 2 to 30 characters |
| Email | email | required, valid format |
| Password | password | required, min. 8 characters |
| Confirm Password | password | required, min. 8 characters |
| Gender | radio | one option required |
| Hobbies | checkbox | optional |
| Country | select | required, placeholder option is not accepted |

## How validation works

Validation is done by the **browser** using HTML attributes: `required`, `minlength`, `maxlength` and `type="email"`.

**Bootstrap only styles the result.** The `was-validated` class on the `<form>` turns on green and red borders based on the `:valid` and `:invalid` states of each field. The `valid-feedback` and `invalid-feedback` blocks are shown or hidden by Bootstrap CSS. For this to work, the feedback block must come right after its input inside the same container.

## Bootstrap components used

- **Navbar**: `navbar`, `navbar-expand-lg`, `navbar-dark`, `bg-dark`, `navbar-toggler`, `collapse navbar-collapse`, `nav-link`, `active`
- **Grid**: `container`, `row`, `col-md-6`
- **Forms**: `form-label`, `form-control`, `form-select`, `form-check`, `form-check-inline`, `form-check-input`, `form-check-label`
- **Validation**: `was-validated`, `valid-feedback`, `invalid-feedback`
- **Buttons**: `btn`, `btn-primary`, `btn-secondary`
- **Utilities**: `mb-3`, `ms-2`, `ms-auto`, `d-block`
- 
## How to run

1. Download or clone the repository.
2. Open `index.html` in a browser.
3. Use the navigation bar to switch between pages.

An internet connection is required because Bootstrap is loaded from a CDN.

## Author

Your name, group and course here.

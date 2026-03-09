# 🔍 Form Validator

A lightweight and reusable JavaScript form validator plugin.

## Features
- 📧 Email format validation
- 📱 Phone number validation (Israel +972 and international formats)
- 🔒 Password validation — min 8 characters, at least 1 number and 1 uppercase letter
- 🔁 Confirm password — checks if passwords match
- 💬 Live validation hints — feedback on every keystroke
- 🟢 Success/error border colors
- 🔌 Reusable — can be connected to any form via selector

## Usage
```javascript
const valid = new Validator({
    selector: '#myform',
    pattern: {
        phone: '',
        email: '',
        password: '',
    },
    method: {
        'email': [['notEmpty'], ['email']],
        'phone': [['notEmpty'], ['pattern', 'phone']],
        'password': [['notEmpty'], ['password']],
        'confirmPassword': [['notEmpty'], ['confirmPassword']]
    }
});

valid.init();
```

## Tech Stack
- HTML
- CSS
- JavaScript

## Getting Started

Just open `index.html` in your browser — no installation needed.
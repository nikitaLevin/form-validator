# 🔍 Form Validator

A lightweight and reusable JavaScript form validator plugin.

## Features
- 📧 Email format validation
- 📱 Phone number validation with custom regex patterns
- 🟢 Green border — valid input
- 🔴 Red border — invalid input
- 🧹 Clears form on successful submit
- 🔌 Reusable — can be connected to any form via selector

## Usage
```javascript
const valid = new Validator({
    selector: '#myform',
    pattern: {
        phone: '',
        email: '',
    },
    method: {
        'phone': [['notEmpty'], ['pattern', 'phone']],
        'email': [['notEmpty'], ['email']]
    }
});

valid.init();
```

## Tech Stack
- HTML
- JavaScript

## Getting Started

Just open `index.html` in your browser — no installation needed.
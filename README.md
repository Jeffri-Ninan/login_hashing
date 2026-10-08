# Minimal Authentication with Password Hashing & JSON Storage

A minimal, single-page web authentication system with Sign In and Sign Up modules, embedded directly in HTML with zero external dependencies.

## Features

- **Embedded Architecture**: Complete HTML, CSS, and JavaScript embedded in a single file (`index.html`).
- **Sign In & Sign Up Modules**: Tabbed navigation between Sign In and Sign Up with clean input fields and password visibility toggles.
- **SHA-256 Cryptographic Hashing**: Uses browser-native Web Crypto API (`crypto.subtle.digest('SHA-256', ...)`) to hash passwords before storing and comparing them.
- **JSON User Storage**: User credentials, hashes, and registration timestamps are serialized and stored as a JSON database in `localStorage`.
- **In-Page Popups**:
  - Pops an **"Account Created Successfully!"** modal popup upon signup.
  - Pops a **"Sign In Successful!"** modal popup upon valid credential authentication.
- **JSON Database Inspector**: Built-in interactive drawer to view, copy, or clear the live stored JSON user records and verify the SHA-256 hashes.

## Getting Started

1. Clone or download this repository:
   ```bash
   git clone https://github.com/Jeffri-Ninan/login_hashing.git
   ```
2. Open `index.html` directly in any modern browser (Chrome, Edge, Firefox, Safari).

## Tech Stack

- **HTML5 & Vanilla CSS3**: Dark minimalist glassmorphic aesthetic with ambient glow and responsive layout.
- **JavaScript (ES6+)**: Pure client-side logic with Web Crypto API and JSON storage handling.

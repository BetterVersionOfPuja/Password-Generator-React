# 🔐 Password Generator (React)

A simple React-based password generator that allows users to create secure, customizable passwords.

---

## 🎯 Purpose of This Project
This project was built to:
- Practice **React Hooks**
- Understand **state management**
- Learn **clipboard access using useRef**
- Build a small real-world utility app

---

## 🛠 Tech Stack
- React (Vite)
- JavaScript (ES6)
- Tailwind CSS

---

## ⚙️ Features
- Generate random passwords
- Adjustable password length (slider)
- Option to include:
  - Numbers
  - Special characters
- Copy password to clipboard

---

## 🧠 React Concepts Used (IMPORTANT)

### useState
Used to manage:
- Password length
- Number toggle
- Character toggle
- Generated password

---

### useCallback
Used to:
- Optimize password generation function
- Prevent unnecessary re-creation of functions

---

### useEffect
Used to:
- Automatically generate a new password when:
  - Length changes
  - Options change

---

### useRef
Used to:
- Access password input field
- Select and copy password text to clipboard

---

## 🔐 Password Generation Logic (REVISION POINT)
1. Create an empty string
2. Add numbers if enabled
3. Add special characters if enabled
4. Loop based on selected length
5. Pick random characters using `Math.random()`
6. Store result in state

---

## 📋 Copy to Clipboard
Uses browser Clipboard API:
```js
navigator.clipboard.writeText(password)

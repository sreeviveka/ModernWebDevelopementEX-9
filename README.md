# Exp 9 – React Lab Exercise: React Fragments

## NAME: V.S.SREE VIVEKA 
## REG NO: 2305001031 

## Aim
To understand and implement React Fragments to group multiple JSX elements without creating unnecessary HTML elements in the DOM.

## Objectives
- Understand the concept of React Fragments.
- Use Fragment shorthand syntax.
- Use the explicit Fragment syntax.
- Group multiple JSX elements without an extra DOM node.
- Understand the difference between Fragments and div elements.

## Program

### Step 1: Create a React Project

```bash
npm create vite@latest react-fragments
cd react-fragments
npm install
npm run dev
```

Select React as the framework and JavaScript as the variant.

### Step 2: App.jsx – Using Fragment Shorthand

```jsx
function Student() {
  return (
    <>
      <h2>Student Details</h2>

      <h3>Name: Sree Viveka</h3>

      <p>Register Number: 2305001031</p>

      <p>Department: Computer Science and Engineering</p>
    </>
  );
}

function App() {
  return (
    <>
      <h1>College Information System</h1>

      <Student />
    </>
  );
}

export default App;
```

### Step 3: Using Explicit Fragment Syntax

```jsx
import { Fragment } from "react";

function Student() {
  return (
    <Fragment>
      <h2>Student Details</h2>
      <p>Name: Sree Viveka</p>
      <p>Department: CSE</p>
    </Fragment>
  );
}

function App() {
  return (
    <Fragment>
      <h1>College Information System</h1>
      <Student />
    </Fragment>
  );
}

export default App;
```

## Output

### Fragment Shorthand Syntax
<img width="1090" height="527" alt="WhatsApp Image 2026-11-11 at 8 50 12 AM" src="https://github.com/user-attachments/assets/dd8a030c-19fc-47f9-a35c-28b88d2da79a" />

### Explicit Fragment Syntax
<img width="1088" height="528" alt="WhatsApp Image 2026-11-11 at 8 48 34 AM" src="https://github.com/user-attachments/assets/b396d016-8047-4b57-91a5-4196b363f2ee" />

## Result

Thus, React Fragments were successfully implemented using shorthand and explicit syntax to group multiple JSX elements without creating unnecessary DOM elements.

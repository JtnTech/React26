# React + Vite Setup Guide 🚀

## 1. Check Node.js Installation

```bash
node -v
npm -v
```

If both commands show versions, Node.js and npm are installed.

---

## 2. Create a React Project

```bash
npm create vite@latest  ## /without folder name , later it will ask for folder name.
OR
npm create vite@latest reactjune ## /thats why we written folder name in single line command , 'reactjune' is a folder name. 
```

Select:

```text
Framework: React
Variant: JavaScript
```

---

## 3. Move Into Project Folder

```bash
cd reactjune
```

### What is `cd`?

`cd` = Change Directory

Example:

```bash
cd reactjune
```

Moves you inside the `reactjune` folder.

---

## 4. Install Dependencies

```bash
npm install
```

or

```bash
npm i
```

### What does it do?

Reads `package.json` and downloads all required packages into:

```text
node_modules/
```

---

## 5. Start Development Server

```bash
npm run dev
```

Output:

```text
Local: http://localhost:5173/
```

Open that URL in your browser.

---

# Useful Terminal Commands

## Create Folder

```bash
mkdir project
```

Creates a folder named `project`.

---

## Enter Folder

```bash
cd project
```

Moves inside the folder.

---

## Go Back One Folder

```bash
cd ..
```

Example:

```text
D:\code\reactjune
        ↓
D:\code
```

---

## Show Files

Windows:

```bash
dir
```

Mac/Linux:

```bash
ls
```

Shows files and folders in current directory.

---

## Current Location

Windows PowerShell:

```bash
pwd
```

Shows current folder path.

---

# Important npm Commands

## Install Package

```bash
npm i react-router-dom
```

Installs React Router.

---

## Install Multiple Packages

```bash
npm i axios react-router-dom
```

---

## Remove Package

```bash
npm uninstall axios
```

---

## Start Project

```bash
npm run dev
```

Runs Vite development server.

---

## Build Project

```bash
npm run build
```

Creates production build.

---

## Preview Build

```bash
npm run preview
```

Preview production build locally.

---

# React Project Structure

```text
reactjune/
│
├── node_modules/
├── public/
├── src/
│   ├── App.jsx
│   ├── main.jsx
│   └── COMPONENT/
│       └── Text.jsx
│
├── package.json
├── vite.config.js
└── index.html
```

---

# React Execution Flow

```text
index.html
    ↓
main.jsx
    ↓
App.jsx
    ↓
Text.jsx
```

React starts from `main.jsx`.

---

# Import Example

## Text.jsx

```jsx
function Text() {
  return <h1>Hello React</h1>;
}

export default Text;
```

## App.jsx

```jsx
import Text from "./COMPONENT/Text";

function App() {
  return (
    <>
      <Text />
    </>
  );
}

export default App;
```

---

# Most Used Commands (Remember These)

```bash
mkdir project
cd project

npm create vite@latest myapp
cd myapp

npm i
npm run dev
```

These are the commands you'll use almost every day while learning React.


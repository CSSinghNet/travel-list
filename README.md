# ✈️ React Travel List App -- README

This project demonstrates core React concepts by building a Travel List
application where users can add, manage, and organize travel items.

------------------------------------------------------------------------

## 📌 Features Implemented

-   Form handling in React
-   Event handling
-   Props usage
-   Passing data between components
-   Component separation into different files
-   Clean project structure

------------------------------------------------------------------------

## 🧾 1. Form Handling in React

A form is used to capture user input such as travel item name and
quantity.

### Example:

``` jsx
function AddItem({ onAddItem }) {
  const handleSubmit = (e) => {
    e.preventDefault();
    // logic to add item
  };

  return (
    <form onSubmit={handleSubmit}>
      <input type="text" placeholder="Enter item" />
      <button>Add</button>
    </form>
  );
}
```

------------------------------------------------------------------------

## ⚡ 2. Event Handling

React uses synthetic events to handle user actions like clicks and form
submissions.

### Example:

``` jsx
<button onClick={handleClick}>Add Item</button>
```

Events handled: - onSubmit - onClick - onChange

------------------------------------------------------------------------

## 📦 3. Props in React

Props are used to pass data from parent to child components.

### Example:

``` jsx
function Item({ name }) {
  return <p>{name}</p>;
}
```

------------------------------------------------------------------------

## 🔁 4. Passing Data Between Components

Data is passed from parent → child using props, and child → parent using
callback functions.

### Example:

``` jsx
function App() {
  const handleAddItem = (item) => {
    console.log(item);
  };

  return <AddItem onAddItem={handleAddItem} />;
}
```

------------------------------------------------------------------------

## 🧩 5. Component Separation

Components are moved into separate files for maintainability and
scalability.

### Project Structure:

    src/
     ├── App.js
     ├── components/
     │    ├── logo.js
     │    ├── list.js
     │    ├── forms.js

Benefits: - Reusable code - Better readability - Easier debugging -
Scalable architecture

------------------------------------------------------------------------

## 🏗️ Application Flow

1.  User enters travel item in form
2.  Form submit triggers event
3.  Data passed to parent component
4.  Parent updates state
5.  Updated list passed back to child via props
6.  UI re-renders with new items

------------------------------------------------------------------------

## 🚀 What I Learned

-   Form creation in React
-   Handling user events
-   Passing data between components
-   Working with props
-   Organizing components into separate files
-   Structuring a real React project

------------------------------------------------------------------------

## 🛠️ Tech Stack

-   ReactJS
-   JavaScript (ES6)
-   JSX
-   CSS

------------------------------------------------------------------------

## 📈 Future Improvements

-   Add delete functionality
-   Add edit/update feature
-   Use useState hook deeply
-   Add local storage persistence
-   Improve UI styling

------------------------------------------------------------------------

## 🙌 Author

Learning React by building practical projects and understanding core
concepts step by step.

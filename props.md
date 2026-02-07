🔹 What are Props in React?

Props (short for properties) are used to pass data from a parent component to a child component.

👉 Props are read-only (immutable)
👉 They help make components reusable

🔹 Why Props are Important?

Share data between components

Make components dynamic

Improve reusability

Follow one-way data flow (parent ➝ child)
Parent Component
function App() {
  return <User name="Azra" age={22} />;
}

Child Component
function User(props) {
  return (
    <h2>
      Name: {props.name}, Age: {props.age}
    </h2>
  );
}

🔹 Props with Destructuring (Best Practice ✅)
function User({ name, age }) {
  return <h2>{name} is {age} years old</h2>;
}

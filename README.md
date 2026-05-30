# React Counter Application

A simple, interactive counter application built using **React Class Components**. This project demonstrates the core concepts of managing component state, handling user events, and updating the user interface dynamically based on user actions.

---

## 🚀 Features & Concepts Covered

### React Class Components
While modern React often uses Functional Components with Hooks, this project utilizes **Class Components** to establish a foundational understanding of:
* Extending the core `Component` class from React.
* Initializing and managing local component **`state`**.
* Using the **`render()`** lifecycle method to return JSX.

### State & Props Management
* **State:** Used internally within the `Counter` component to track the changing `count` value.
* **Props:** Though this specific counter manages internal state, the application structure is set up to allow the parent component (`App`) to seamlessly pass read-only data (props) down to the `Counter` if needed.

---

## 🛠️ Step-by-Step Implementation Detail

### 1. Building the Static Version
The development process began by creating a static layout of the application. 
* Designed the UI container, heading, counter display text, and action buttons using JSX.
* Styled the elements using a companion `index.css` file to ensure a clean, centered interface layout before adding any interactivity.
* Initialized the state with a default value: `state = { count: 0 }`.

### 2. Adding Event Listeners
To make the application interactive, React event listeners were attached directly to the JSX elements:
* An `onClick` listener was added to the **Increase** button, mapping to the `this.onIncrement` method.
* An `onClick` listener was added to the **Decrease** button, mapping to the `this.onDecrement` method.
* *Note:* Methods are defined as arrow functions (`onIncrement = () => {}`) to automatically bind the `this` context to the component class.

### 3. Updating Count Based on User Actions
State updates in React are asynchronous and must never be mutated directly. The counter updates state safely by using the **updater function form** of `this.setState()`:
* **Increment:** Accesses `prevState.count`, logs the prior value to the console for debugging, and returns `{ count: prevState.count + 1 }`.
* **Decrement:** Accesses `prevState.count` and returns `{ count: prevState.count - 1 }`.

---

# Step 1:
Open your terminal and navigate to your project directory
cd path/to/your/project-folder

# Step 2:
Install all required project dependencies
npm install

# Step 3:
Start the local development server
npm start
# (Note: Use "npm run dev" if your project template uses Vite instead of Create React App)

# Step 4:
Open your web browser and view the application at: http://localhost:3000  (or http://localhost:5173 for Vite)


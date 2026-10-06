To accelerate the development process and resolve specific logic blockers during the migration to Redux Toolkit, I utilized AI (Gemini) during this sprint. Below is the log of the prompts used:

### Prompt 1
**Tool Used:** Gemini  
**Prompt:** "How do I set up a Redux Toolkit store in a React Vite project to replace my existing Context API setup?"  
**Help Received:** Understood the core boilerplate required for RTK, including how to configure the central store using `configureStore` and how to globally wrap the application using the `<Provider>` component in `main.jsx`.

### Prompt 2
**Tool Used:** Gemini  
**Prompt:** "How do I create Redux slices for managing a shopping cart and product category filters?"  
**Help Received:** Learned the structure of `createSlice()`. Understood how to define the initial state and write reducer functions like `addToCart` (to manage items and quantities) and `setCategory` (for filtering logic).

### Prompt 3
**Tool Used:** Gemini  
**Prompt:** "How can I dynamically calculate the total number of items in my cart and display it in the Navbar using Redux state?"  
**Help Received:** Learned how to effectively use the `useSelector` hook to extract cart data from the global store, and how to apply the JavaScript `.reduce()` method on the cart array to calculate the live total item count for the header.

### Prompt 4
**Tool Used:** Gemini  
**Prompt:** "When I click the 'Add to Cart' button on my product card, it successfully dispatches the action but also accidentally navigates me to the product details page. How do I fix this?"  
**Help Received:** Understood the concept of JavaScript event bubbling. Learned to apply `e.stopPropagation()` inside the button's click handler to isolate the dispatch action and prevent the parent card's navigation event from triggering.

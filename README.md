# Tasks to Complete

---

## General Setup
- [x] Clone repo
- [x] Configure GitHub Pages

---

<details>
  <summary>Task 1: ProductList Component Layout</summary>

- [x] Display the Plant Array
- [x] Display Plant Details within a `<div>` tag with class name `product-grid`
- [x] Display an **Add to Cart** button for each plant
- [x] Create a state variable named `addedToCart` using the `useState` hook to track which products are added to the cart
- [x] Implement **Add to Cart** functionality
- [x] `handleAddToCart()` function will:
   - Carry the details of the selected plant
   - Add the plant details to the cart at a global level using `CartSlice.jsx`
- [x] Save your changes and push the code to your GitHub repository

</details>

---

<details>
  <summary>Task 2: State management using Redux</summary>

- [X] Define Reducer Functions
    - Now implement the reducer property of the slice for adding, removing, and updating the number of items in the cart.
    - These reducer functions will be called when user wants to add or remove the quantity of plants within the cartItems component.
    - The addItem() reducer adds a new plant item to the items array which you initialized in the previous step.
    - The addItem() function should get called when the user selects an Add to cart on the plant listing page. Subsequently, the handleAddToCart() gets called which has the plant type as a parameter.
    - The handleAddToCart() function will then dispatch the plant details to the addItem() reducer function in CartSlice.jsx.
    - Now you need to complete code for the removeItem() and updateQuantity() reducers.
    - removeItem(): This reducer removes an item from the cart based on its name and gets called when the user wants to remove products from the cart.
    - updateQuantity(): To create this function, start by extracting the item's name and amount from the action.payload. Then, look for the item in the state.items array that matches the extracted name. If the item is found, update its quantity to the new amount provided in the payload. This ensures the item’s quantity is correctly updated based on the action.
- [X] Handle Actions
    - Export the action creators, addItem() to use in ProductList.jsx, removeItem(), and updateQuantity(), to use in the CartItem.jsx.
    - Also export the reducer as the default to use in store.js.
    - Make sure you save these changes by pushing your code to your GitHub repository.
</details>

---

<details>
  <summary>Task 3: Cartitems component</summary>

- [ ] Calculate the total for all items in the cart.
- [ ] Calculate the subtotal for each plant type in the cart.
- [ ] Continue shopping
- [ ] Increment and decrement the number of each plant type in the cart
- [ ] Remove (delete) a plant type from the cart altogether.

</details>

# Buybusy2
## Problem Statement
BuyBusy is a web application for the customers of an e-commerce business.

### Goal
Refactor the E-Commerce site to use Redux Toolkit for global state management and a centralized store to persist the state.

### Acceptance criteria
1. The app must implement global state management using Redux Toolkit.
2. The code quality of the React app must be of a high standard, with proper documentation of code and functionality.
3. There must be no cheating or copy-pasting of code from other sources, and all code must be original and developed specifically for this project.

### Tasks
1. Integrate Redux Toolkit for global state management and create a centralized store to persist the state.
2. Create the required reducers and actions for mutating the state.
3. Create a login page that allows existing users to login into your app.
4. Create asynchronous thunks for performing asynchronous logic(Login/Signup, Adding/Removing product in cart etc.)
5. Utilize extraReducers() to update the state based on the promise returned by asynchronous thunks, which include Pending, Fulfilled, and Rejected actions.
6. Update the components of the e-commerce app to use the new Redux Toolkit state management system.
7. Additionally, you can add the following functionality to the project to maximize your score:
  - Create a sidebar to filter the products based on product price and categories on the HomePage. The search and filter should be applied to the products simultaneously.
  - Add and use functions like createSelector() and createEntityAdapter() for better performance. createSelector() creates memoized selectors, which can cache the result of a calculation and only recompute it if the input data changes. createEntityAdapter() creates a normalized state structure for storing collections of entities.

### Hints

1. Use separate slices to manage the user authentication state and product state. For example, the authentication slice may have actions for handling login success, logout, setting the error message, etc.
2. Use createAsyncThunk() function to work with asynchronous code and API requests.
3. Create a function that can apply both search and filters at the same time. The function should have distinct logic for filtering based on category, price range, and search terms.
4. To use the useSelector() hook - Define a function to return the state and pass it to useSelector(). It automatically subscribes to the store and returns the selector function's result when the store updates. Utilize the returned value to update the UI

## Evaluation Criteria
Your project will be evaluated on following parameters -
- USAGE OF SLICES, CREATEASYNCTHUNK() AND EXTRAREDUCERS() FUNCTION
(Max Score 50): <br>
Usage of the createSlice(), Usage of createAsyncThunk() function to implement asynchronous logic, Usage of extraReducers()
- USAGE OF SELECTOR FUNCTIONS WITH USESELECTOR() AND USEDISPATCH() HOOKS
(Max Score 20): <br>
Products are retrived on app mount by dispatching action inside of useEffect() hook and Selector functions are used to reduce the redundancy inside useSelector() hooks.
- NAMING CONVENTIONS AND FOLDER STRUCTURE
(Max Score 10): <br>
Naming of variables and functions should match the conventions like suffixing "Slice" while creating slice etc. All the related files must be maintained in the dedicated folders.
- CODE QUALITY
(Max Score 5): <br>
Clear separation of concerns, with components handling UI and Redux handling state management.
- COMMENTS AND DOCUMENTATION
(Max Score 5): <br>
Solution code is documented and explained with comments along with a Readme.md file
- USAGE OF ADVANCE HOOKS, INNOVATIVE UI AND IMPLEMENTATION OF ADDITIONAL TASKS
(Max Score 10): <br>
Implementation of sidebar for filtering of products and Memoizing expensive selectors to reduce the number of recomputations.

## Hosted Link
https://tangerine-gingersnap-3c8b63.netlify.app/

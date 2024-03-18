# reactInterview


## 1.how to use redux, useContext, useReducer? If you were the architect, which tech stack would you choose and why
Redux:
Purpose: Redux is a predictable state container for JavaScript applications, commonly used with React. It provides a centralized store to manage the entire application's state, making state changes predictable and manageable.
Usage: To use Redux in a React application, you'd create a store, define reducers to manage different parts of the state, dispatch actions to update the state, and connect components using connect (for class components) or useSelector and useDispatch hooks (for functional components).

useContext:
Purpose: useContext is a React hook that allows components to access values stored in the context without explicitly passing props through every level of the component tree. It's ideal for passing down global data that multiple components need.
Usage: Create a context using createContext, provide it at a higher level using Provider, and consume the context value in nested components using useContext.

useReducer:
Purpose: useReducer is a React hook that is an alternative to useState for managing more complex state logic in functional components. It uses a similar pattern to Redux reducers.
Usage: Define a reducer function that specifies how the state should change in response to actions. Then, use useReducer to manage state and dispatch actions.

When chosing between them, consider 
Application Complexity:
For smaller applications with simpler state management needs, using useContext and useReducer could suffice, avoiding the additional overhead of setting up Redux.
For large-scale applications with complex state management requirements, especially those with multiple components needing shared state or intricate interactions, Redux might offer better organization and scalability.
Performance Considerations:
For performance-critical applications, minimizing unnecessary global state management might favor the use of more localized state management approaches like useContext and useReducer.

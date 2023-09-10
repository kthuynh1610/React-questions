# React-questions

1. What is React? 
   React( known as Reactjs or React.js) is an open-source Javascript library that used for building composable user interfaces specially used for single page application.
2. What is main features of React?
   - Using JSX (Javascript xml) syntax, a syntax extension of JS that allow user can use HTML tag into JS
   - Using Virtual DOM instead of real DOM - because virtual DOM works fast which mean Virtual DOM only change individual elements not re-render the whole DOM tree. 
   - Support server side rendering which is useful for SEO(Search engine optimizations) 
   - Follows one-way data binding: which mean they gives better control to the user throughout the application
   - Uses re-usable UI components to develop the view
3. What is class component and function component? When to use?
   Class component is a only way(before React 16.8) to track state and life cycle of react component. 

   Function component before is considered as a state-less component, but after React 16.8 by additional of Hooks, function component now can track state and life cycle of React Component which more useful 
  
   2 reasons to use class component over functional component (before 16.8) 
   - track state and lifecycle method of react component
   - If you need a React functionality whose Function component equivalent is not present yet, like Error Boundaries. 
   But after 16.8 by additional of Hooks, now functional component can solve all these problems
   Benefit of use Functional Component, 
   - Easy to write, understand and test
   - Faster to write, maintain
   - Can avoid this keyword that sometime confuses.
    



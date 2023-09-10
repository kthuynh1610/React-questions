![image](https://github.com/kthuynh1610/React-questions/assets/55730048/d54aebb8-d3c9-422b-89f0-786eb4f0d7e3)# React-questions

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
 4. What is the difference between DOM and Virtual DOM?
    Virtual DOM basically is a copy version of DOM but difference with DOM, whenever any underlying data changes, the entire UI tree re-render then compare with real DOM, if the changes is applied the real DOM      will update immediately. 
   	•  Virtual DOM update faster since they only update small node in node tree => improve performance
   	• DOM manipulation is easy (real DOM is expensive) 
   	• Update direct to JSX if element update ( DOM will create new DOM if elements update)
 5. What is the difference between Shadow DOM and Virtual DOM? 
    Shadow DOM is a browser technology designed for primarily scoping variables and CSS in web components 
    Virtual DOM is a concept implemented by libraries Javascript on top of browser APIs
 6. What is props and state, difference? 
    Props (properties) is a plain object of Javascipt (contain single values or set of values) that used to pass to components on creation similiar to HTML tag attributes. 
    Purpose: 
   	- Pass custom data to child component
   	- Trigger state change
    State is a a plain object that hold some information that may change over lifetime of the component. The key point is whenever the state change the components will re-render.
   
    State and Props are plain object of Javascipt that manage the data of components but the purpose in use is different.
    State is managed by the component itself and can be "updated" by setState function. Unlike State, Props are passed by component by its parent and understand as "read-only" which mean they cant be 
    modified by the component itself. 
 7. Why should we not update the state directly?
    By using setState, whenever the state change, the component itself will re-render in-order to update virtual DOM, if update the state directly, component won't re-render
 8. What is ref and purpose of using refs? 
    Ref or useRef is a react hook that allow you to reference value that's not needed to re-render. 

    Purpose: 
   - use it to not trigger a re-render => refs is good for value that doesnt affect the visual output of your component. 
   - use to store information between re-render => good for application such as save value of a stopwatch
   - the information is local to each copy of your component
 9. What is reconciliation?
    Reconciliation is a process that React uses to update DOM and makes React work faster. 
    Process is : Component changes => use diffing algorithm to compare DOM vs Virtual DOM => whether changes => update DOM with that nodes change.
10. What are fragments in React?
    Fragments are tag that used to group a list of children without adding a extra node into DOM => this make React perform faster instead of use Div.
11. Why fragment are bteer than container div?
     Fragment are a bit faster and use less memory by not creating an extra DOM node, This only has a real benefit if you come to large and deep trees project. => main reason
     
12. What is Higher Order Component? (HOC)
    HOC is simply take in a component and return a new component, which mean this component is a re-usable component
13. What is stateless and stateful component?
    Stateless component is a component that their behaviour is independent of its state, opposite with Stateless, Stateful is a component that dependent on the state.
14. What is synthetic events in React? 
    SyntheticEvent is a cross-browser wrapper around the browser's native event. Its API is same as the browser's native event, including stopPropagation() and preventDefault(), except the events work            identically across all browsers. The native events can be accessed directly from synthetic events using nativeEvent attribute.\
15. What is 'key' prop and what is the benefit of using it in arrays of element?
    Key is a specical prop in array function helper : map. Key prop helps React can track or identity whether item changed, added or removed.
16. What are the advantages of React?
    Increases the application's performance with Virtual DOM.
    JSX makes code easy to read and write.
    It renders both on client and server side (SSR).
    Easy to integrate with frameworks (Angular, Backbone) since it is only a view library.
    Easy to write unit and integration tests with tools such as Jest.
17. What are the limitations of React?
    React is just a view library, not a full framework.
    There is a learning curve for beginners who are new to web development.
    Integrating React into a traditional MVC framework requires some additional configuration.
    The code complexity increases with inline templating and JSX.
    Too many smaller components leading to over engineering or boilerplate.
18. What is the purpose of render method of react-dom?
    This method is used to render a React element into the DOM in the supplied container and return a reference to the component. If the React element was previously rendered into container, it will perform      an update on it and only mutate the DOM as necessary to reflect the latest changes.

   ReactDOM.render(element, container, [callback])

   If the optional callback is provided, it will be executed after the component is rendered or updated












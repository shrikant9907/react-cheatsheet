# Basic of React JS for Interview 


## What is React JS? and Why we use it? 
- Open source Javascript Library
- It was developed by a developer "Jordan Walk" from facebook.
- Reusable Components
- Huge Community of Developers
- Single Page Application (SAP)

## JSX
- Javascript XML
- Allow us to use HTML like syntax in JavaScript
- Browser can not understand JSX. It uses a compilter for that called Babel.
(Babel converted JSX to JavaScript)

## Pass Data to Component
- Using Props
- Context API
-- It allows us to pass the data to component without props drilling, It uses context.provider to provide the data and context.consumer to receive the data.
- Context API is added in the version 16.3
- We can create a context object using React.createContext(DefaultValue)
- useContextHook -. 16.8
```
const values = React.useContext(Object)
```

## State VS Props
- Read and Update | readonly
- Mutable | immutable

## React Fragment
- Used for grouping of element without using any extra node in the DOM


## Keys
- Unique value that we pass to the component
- React using keys to update or delete an element
- It increses the performaces 
- Keys are used with .map function

## Ref
- Ref is the refereces to the DOM element
- Eg. Foucs, Text Selection 
- Introduced in the version 16.3 
- Forward Ref: to pass the reference of an element to another element
- useRef: Hook and used for passing the refereces to a variable
```
const Ref = useRef();
```

## useEffect
- performing the side effect in the component.
- side effects are the operations that are performed by the outside world like get & post request by the API's or working with the Browser API like window.navigation etc.
- useEffect is a Hook --- > 16.8
- It works like the life cycle methods in of the class components eg. componentDidMount, componentDidUpdate, ComponentWithUnmount,

## useCallback
- It returns memoized function 
```
const todo = useCallback(()=> {
  setTodo((t)=> [...t,'new'])
}, [todo])
```

## useMemo
- Memoized Value
- Caching a vlaue that dones not need to recalculate
- Improves performance
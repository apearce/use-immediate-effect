# use-immediate-effect
Because sometimes you want your effects to run right away

## Installation
`npm i use-immediate-effect`

## useImmediateEffect
### Usage
When using `useEffect` or `useLayoutEffect`, the execution of the passed in function is deferred. There may be times when you want it to execute immediately, which is what `useImmediateEffect` does. The signature is the same as `useEffect` and `useLayoutEffect`.

```jsx
import useImmediateEffect from 'use-immediate-effect';

function SomeComponent(props) {
    ...
    useImmediateEffect(() => {
        ...
        return () => {
            ...
        };
    }, [someDeps]);
    ...
}
```
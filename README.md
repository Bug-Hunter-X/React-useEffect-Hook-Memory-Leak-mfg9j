# React useEffect Hook Memory Leak

This example demonstrates a common error in React's `useEffect` hook that can lead to memory leaks.  The component sets up an interval to update a counter, but fails to properly clear the interval when the component unmounts. This is further exacerbated by incorrect variable scope management of `intervalId`. 

The solution showcases the correct implementation of the cleanup function within the `useEffect` hook to prevent memory leaks.
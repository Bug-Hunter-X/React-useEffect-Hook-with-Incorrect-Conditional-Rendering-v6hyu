# React useEffect Hook with Incorrect Conditional Rendering
This example demonstrates a common error in React's `useEffect` hook where the conditional logic within the effect is not correctly handling the initial render, potentially leading to unexpected behavior or even an infinite loop. 

## Problem
The provided code demonstrates how useEffect does not execute on the initial render when count is 0. This leads to an effect that only activates when the count is greater than 0, missing the first render where the count is initialised to 0.

## Solution
The solution illustrates how to handle the initial render and subsequent renders correctly. The code now uses the `count` value to trigger the effect, thus updating only when count changes and covering the initial render where `count` is 0.
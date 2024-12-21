# Unexpected behavior with string | null type and undefined value
This example demonstrates an unexpected behavior when using 'undefined' with a string | null type in TypeScript.

## Bug Description
TypeScript's type guards don't always handle optional parameters gracefully. When you have a function expecting a string or null, passing 'undefined' can lead to runtime errors or unexpected behavior, even though 'undefined' might seem logically compatible with the null check. 

## Solution
The solution is to explicitly handle the 'undefined' case in your type guard, either by adding it to the type definition or using a more robust check in your conditional statements.
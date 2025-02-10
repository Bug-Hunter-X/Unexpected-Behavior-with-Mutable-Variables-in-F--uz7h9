# Unexpected Behavior with Mutable Variables in F#

This example demonstrates a common issue when working with mutable variables in F#.  Because F# mutable variables are passed by reference, directly swapping their values within a function affects the original variables unexpectedly. The `swap` function intends to swap the values of `x` and `y`, but it modifies the global variables as well. 

## How to Reproduce

1. Compile and run the `bug.fs` file.
2. Observe that the output is not what you would expect for a simple swap operation.
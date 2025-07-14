

- TVMLKit JS
- TVMLKit JS Functions
-  clearTimeout 

Function

# clearTimeout

Stops the function associated with the identifier from executing.

tvOS 9.0+

``` source
void clearTimeout(
    in String timeoutID
);
```

## Parameters 

`timeoutID`  

A string identifying the timeout to clear.

## Discussion

This function stops the function associated with the identifier created by the setTimeout function from executing.

## See Also

### Automating Function Timing

setInterval

Repeatedly executes a given function at the given time interval.

clearInterval

Stops the function associated with the identifier from repeating.

setTimeout

Executes a given function after a set amount of time.


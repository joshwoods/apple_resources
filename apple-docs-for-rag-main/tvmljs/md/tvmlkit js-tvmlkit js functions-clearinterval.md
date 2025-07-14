

- TVMLKit JS
- TVMLKit JS Functions
-  clearInterval 

Function

# clearInterval

Stops the function associated with the identifier from repeating.

tvOS 9.0+

``` source
void clearInterval(
    in String intervalID
);
```

## Parameters 

`intervalID`  

A string identifying the interval to clear.

## Discussion

This function stops the function associated with the identifier created by the setInterval function from executing.

## See Also

### Automating Function Timing

setInterval

Repeatedly executes a given function at the given time interval.

setTimeout

Executes a given function after a set amount of time.

clearTimeout

Stops the function associated with the identifier from executing.




- TVMLKit JS
- TVMLKit JS Functions
-  setInterval 

Function

# setInterval

Repeatedly executes a given function at the given time interval.

tvOS 9.0+

``` source
String setInterval(
    in Function func, 
    in Integer time
);
```

## Parameters 

`func`  

The function to be executed.

`time`  

An integer value that defines, in milliseconds, how often the function is to repeat.

## Return Value

Returns a string containing an identifier for the interval just set.

## Discussion

Pass the identifier created by this function to the clearInterval function to stop the designated function from executing.

## See Also

### Automating Function Timing

clearInterval

Stops the function associated with the identifier from repeating.

setTimeout

Executes a given function after a set amount of time.

clearTimeout

Stops the function associated with the identifier from executing.


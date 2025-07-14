

- TVMLKit JS
- TVMLKit JS Functions
-  setTimeout 

Function

# setTimeout

Executes a given function after a set amount of time.

tvOS 9.0+

``` source
String setTimeout(
    in Function func, 
    in Integer time
);
```

## Parameters 

`func`  

The function to be executed.

`time`  

An integer value that defines, in milliseconds, how long until the function is executed.

## Return Value

Returns a string containing an identifier for the timeout just set.

## Discussion

Pass the identifier created by this function to the clearTimeout function to stop the designated function from executing.

## See Also

### Automating Function Timing

setInterval

Repeatedly executes a given function at the given time interval.

clearInterval

Stops the function associated with the identifier from repeating.

clearTimeout

Stops the function associated with the identifier from executing.


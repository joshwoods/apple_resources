

- DriverKit
-  IODispatchLogFunction 

Type Alias

# IODispatchLogFunction

A function that logs content.

DriverKitiOSiPadOSmacOS

``` source
typedef int (*)(const char *, ...) IODispatchLogFunction;
```

## Parameters 

`format`  

The C string to add to the log.

## See Also

### Logging Dispatch Information

Log

Log the current execution context with respect to any queues the current thread holds.


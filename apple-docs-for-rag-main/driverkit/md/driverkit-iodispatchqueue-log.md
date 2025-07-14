

- DriverKit
- IODispatchQueue
-  Log 

Static Method

# Log

Log the current execution context with respect to any queues the current thread holds.

DriverKitiOSiPadOSmacOS

``` source
static void Log(const char * message, IODispatchLogFunction output);
```

## Parameters 

`message`  

A C string that contains the message to add to the log file.

`output`  

The function address to use for logging the content. The address of IOLog is suitable for use.

## See Also

### Logging Dispatch Information

IODispatchLogFunction

A function that logs content.


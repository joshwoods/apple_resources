

- DriverKit
-  IODispatchFunction 

Type Alias

# IODispatchFunction

A C-style function to execute on a dispatch queue.

DriverKitiOSiPadOSmacOS

``` source
typedef void (*)(void *) IODispatchFunction;
```

## Parameters 

`context`  

A pointer to contextual data that you need to perform any tasks. You specify the pointer to this data when scheduling the function for execution.

## See Also

### Executing a Task Asynchronously

DispatchAsync

Schedule a block for asynchronous execution on the current queue.

DispatchAsync_f

Schedule a C-style function for asynchrous execution on the current queue.

IODispatchBlock

A block to execute on a dispatch queue.


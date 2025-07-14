

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IODispatchQueue
-  DispatchAsync_f 

Instance Method

# DispatchAsync_f

Schedule a C-style function for asynchrous execution on the current queue.

DriverKitKernelDriverKit 19.0+macOS 10.15.2+

``` source
void DispatchAsync_f(void *context, IODispatchFunction function);
```

## Parameters 

`context`  

A pointer to contextual data that you want to pass to the function.

`function`  

The function to execute on the queue.

## Discussion

This method schedules the function for execution on the queue and returns immediately, without waiting for execution of the function to begin. The system retains the queue until the function completes.

## See Also

### Executing a Task Asynchronously

IODispatchBlock

A block to execute on a dispatch queue.

IODispatchFunction

A C-style function to execute on a dispatch queue.

- DispatchAsync

Schedule a block for asynchronous execution on the current queue.


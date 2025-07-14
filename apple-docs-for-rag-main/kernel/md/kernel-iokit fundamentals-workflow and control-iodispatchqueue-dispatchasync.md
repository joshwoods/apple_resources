

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IODispatchQueue
-  DispatchAsync 

Instance Method

# DispatchAsync

Schedule a block for asynchronous execution on the current queue.

DriverKitKernelDriverKit 19.0+macOS 10.15.2+

``` source
void DispatchAsync(IODispatchBlock block);
```

## Parameters 

`block`  

The block to execute on the queue.

## Discussion

This method schedules the block for execution on the queue and returns immediately, without waiting for execution of the block to begin. The system retains the queue until the block completes.

## See Also

### Executing a Task Asynchronously

IODispatchBlock

A block to execute on a dispatch queue.

IODispatchFunction

A C-style function to execute on a dispatch queue.

- DispatchAsync_f

Schedule a C-style function for asynchrous execution on the current queue.


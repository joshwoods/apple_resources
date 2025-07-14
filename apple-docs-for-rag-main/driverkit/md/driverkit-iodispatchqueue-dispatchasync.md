

- DriverKit
- IODispatchQueue
-  DispatchAsync 

Instance Method

# DispatchAsync

Schedule a block for asynchronous execution on the current queue.

DriverKitiOSiPadOSmacOS

``` source
void DispatchAsync(IODispatchBlockblock);
```

## Parameters 

`block`  

The block to execute on the queue.

## Discussion

This method schedules the block for execution on the queue and returns immediately, without waiting for execution of the block to begin. The system retains the queue until the block completes.

## See Also

### Executing a Task Asynchronously

DispatchAsync_f

Schedule a C-style function for asynchrous execution on the current queue.

IODispatchBlock

A block to execute on a dispatch queue.

IODispatchFunction

A C-style function to execute on a dispatch queue.


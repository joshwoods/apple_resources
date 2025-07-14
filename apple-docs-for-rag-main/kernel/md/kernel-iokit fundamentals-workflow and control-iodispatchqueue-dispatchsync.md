

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IODispatchQueue
-  DispatchSync 

Instance Method

# DispatchSync

Schedule a block for synchronous execution on the current queue.

DriverKitKernelDriverKit 19.0+macOS 10.15.2+

``` source
void DispatchSync(IODispatchBlock block);
```

## Parameters 

`block`  

The block to execute on the queue.

## Discussion

This method schedules the block for execution on the queue and waits for it to complete before returning. The system retains the queue until the block completes.

## See Also

### Executing a Task Synchronously

- DispatchSync_f

Schedule a C-style function for synchronous execution on the current queue.


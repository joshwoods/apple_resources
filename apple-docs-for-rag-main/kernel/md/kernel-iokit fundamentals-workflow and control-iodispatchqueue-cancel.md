

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IODispatchQueue
-  Cancel 

Instance Method

# Cancel

Stops the queue from dequeueing any further tasks, and notifies the specified handler when all in-flight tasks finish.

DriverKitKernelDriverKit 19.0+macOS 10.15.2+

``` source
kern_return_t Cancel(IODispatchQueueCancelHandler handler);
```

## Parameters 

`handler`  

The block to execute when the queue finishes all in-flight work.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see `Error Codes`.

## Discussion

This method asynchronously tells the dispatch queue to stop the execution of queued tasks, and returns immediately. If a task is already executing, that task runs to completion. After all tasks finish, the dispatch queue executes the block in the `handler` parameter.

## See Also

### Stopping the Queue

IODispatchQueueCancelHandler

A block to execute when a canceled dispatch queue stops executing tasks.


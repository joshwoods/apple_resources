

- DriverKit
- IODispatchQueue
-  DispatchSync_f 

Instance Method

# DispatchSync_f

Schedule a C-style function for synchronous execution on the current queue.

DriverKitiOSiPadOSmacOS

``` source
void DispatchSync_f(void * context, IODispatchFunction function);
```

## Parameters 

`context`  

A pointer to contextual data that you want to pass to the function.

`function`  

The function to execute on the queue.

## Discussion

This method schedules the function for execution on the queue and waits for it to complete before returning. The system retains the queue until the function completes.

## See Also

### Executing a Task Synchronously

DispatchSync

Schedule a block for synchronous execution on the current queue.


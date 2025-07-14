

- DriverKit
- IODispatchQueue
-  DispatchSync 

Instance Method

# DispatchSync

Schedule a block for synchronous execution on the current queue.

DriverKitiOSiPadOSmacOS

``` source
void DispatchSync(IODispatchBlockblock);
```

## Parameters 

`block`  

The block to execute on the queue.

## Discussion

This method schedules the block for execution on the queue and waits for it to complete before returning. The system retains the queue until the block completes.

## See Also

### Executing a Task Synchronously

DispatchSync_f

Schedule a C-style function for synchronous execution on the current queue.


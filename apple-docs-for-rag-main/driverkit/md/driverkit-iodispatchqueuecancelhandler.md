

- DriverKit
-  IODispatchQueueCancelHandler 

Type Alias

# IODispatchQueueCancelHandler

A block to execute when a canceled dispatch queue stops executing tasks.

DriverKitiOSiPadOSmacOS

``` source
typedef void (^)(void) IODispatchQueueCancelHandler;
```

## See Also

### Stopping the Queue

Cancel

Stops the queue from dequeueing any further tasks, and notifies the specified handler when all in-flight tasks finish.




- DriverKit
- IODataQueueDispatchSource
-  CheckForWork 

Instance Method

# CheckForWork

Checks for events to handle.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t CheckForWork(bool synchronous);
```

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Don’t override this method or call it from your own code. The dispatch source uses this method internally to check for events.

## See Also

### Performing Internal Tasks

CopyDataAvailableHandler

A private method that the dispatch source uses to detect enqueued data.

CopyDataServicedHandler

A private method that the dispatch source uses to detect dequeued data.

CopyMemory

A private method that the dispatch source uses to copy memory.




- DriverKit
- IODataQueueDispatchSource
-  CopyDataAvailableHandler 

Instance Method

# CopyDataAvailableHandler

A private method that the dispatch source uses to detect enqueued data.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t CopyDataAvailableHandler(OSAction * * action);
```

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Performing Internal Tasks

CopyDataServicedHandler

A private method that the dispatch source uses to detect dequeued data.

CopyMemory

A private method that the dispatch source uses to copy memory.

CheckForWork

Checks for events to handle.


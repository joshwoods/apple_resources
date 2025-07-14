

- DriverKit
- IODataQueueDispatchSource
-  CopyMemory 

Instance Method

# CopyMemory

A private method that the dispatch source uses to copy memory.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t CopyMemory(IOMemoryDescriptor * * memory);
```

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Performing Internal Tasks

CopyDataAvailableHandler

A private method that the dispatch source uses to detect enqueued data.

CopyDataServicedHandler

A private method that the dispatch source uses to detect dequeued data.

CheckForWork

Checks for events to handle.


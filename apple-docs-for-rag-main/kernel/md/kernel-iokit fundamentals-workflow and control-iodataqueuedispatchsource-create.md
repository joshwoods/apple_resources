

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IODataQueueDispatchSource
-  Create 

Type Method

# Create

Creates a dispatch source that you use as a shared-memory data queue.

DriverKitKernelDriverKit 19.0+macOS 10.15.2+

``` source
static kern_return_t Create(uint64_t queueByteCount, IODispatchQueue *queue, IODataQueueDispatchSource **source);
```

## Parameters 

`queueByteCount`  

The size of the queue in bytes.

`queue`  

The dispatch queue to use for executing tasks. Note that the DataAvailable and DataServiced handlers execute on the queue set for the target method of the associated OSAction object, not this queue.

`source`  

A variable for storing the resulting dispatch source object. On success, the returned object has a retain count of 1, and you must release it when finished.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See `Error Codes`.

## See Also

### Configuring the Dispatch Source

- init

Handles the basic initialization of the dispatch source.

- free

Performs any final cleanup for the data-queue dispatch source.


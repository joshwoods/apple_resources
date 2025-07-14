

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IODispatchQueue
-  Create 

Type Method

# Create

Creates a new dispatch queue object.

DriverKitKernelDriverKit 19.0+macOS 10.15.2+

**DriverKit**

``` source
static kern_return_t Create(const IODispatchQueueName name, uint64_t options, uint64_t priority, IODispatchQueue **queue);
```

**macOS**

``` source
static kern_return_t Create(const char *name, uint64_t options, uint64_t priority, IODispatchQueue **queue);
```

## Parameters 

`options`  

No options are currently defined. Specify `0` for this parameter.

`priority`  

No priorities are currently defined. Specify `0` for this parameter.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see `Error Codes`.

## Discussion

Creates a new dispatch queue object. All queues are currently serial, executing one block at time in FIFO order. The new object has retain count of 1 and should be released by the caller.

## See Also

### Creating a Dispatch Queue

- init

Initializes the dispatch queue object.

- free

Performs any final cleanup for the dispatch queue object.


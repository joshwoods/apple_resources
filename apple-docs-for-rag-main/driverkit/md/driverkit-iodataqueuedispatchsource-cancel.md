

- DriverKit
- IODataQueueDispatchSource
-  Cancel 

Instance Method

# Cancel

Cancels all callbacks from the dispatch source.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t Cancel(IODispatchSourceCancelHandlerhandler);
```

## Parameters 

`handler`  

The handler block to call after any in-flight callbacks finish executing.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

After cancelling a dispatch source, you cannot reactivate it.

## See Also

### Starting and Stopping the Dispatch Source

SetEnableWithCompletion

Controls the enable state of the interrupt source.


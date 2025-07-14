

- DriverKit
- IODispatchSource
-  Cancel 

Instance Method

# Cancel

Cancel all callbacks from the dispatch source.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t Cancel(IODispatchSourceCancelHandlerhandler);
```

## Parameters 

`handler`  

The handler block to execute after the dispatch source finishes any in-flight callbacks.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Subclasses must provide an implementation of this method. After cancellation, the dispatch source can only be freed. It cannot be reactivated.

## See Also

### Configuring the Dispatch Source

init

Handles the basic initialization of the dispatch source.

free

Performs any final cleanup for the dispatch source.


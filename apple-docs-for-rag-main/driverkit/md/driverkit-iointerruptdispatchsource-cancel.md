

- DriverKit
- IOInterruptDispatchSource
-  Cancel 

Instance Method

# Cancel

Cancels all callbacks from the event source.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t Cancel(IODispatchSourceCancelHandlerhandler);
```

## Parameters 

`handler`  

The handler block to execute after any interrupt callbacks finish.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

After cancellation, the source can only be freed. It cannot be reactivated.

## See Also

### Starting and Stopping the Interrupt Source

SetEnableWithCompletion

Enables or disables the delivery of interrupts.

IODispatchSourceCancelHandler

A block to execute when a canceled dispatch source stops executing tasks.




- DriverKit
- IOInterruptDispatchSource
-  SetEnableWithCompletion 

Instance Method

# SetEnableWithCompletion

Enables or disables the delivery of interrupts.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t SetEnableWithCompletion(bool enable, IODispatchSourceCancelHandlerhandler);
```

## Parameters 

`enable`  

A Boolean value that indicates whether to enable the dispatch source. Specify `true` to enable the dispatch source, or `false` to disable it.

`handler`  

An optional block to execute when disabling the dispatch source. The dispatch source executes it after all pending interrupts finish executing.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Starting and Stopping the Interrupt Source

Cancel

Cancels all callbacks from the event source.

IODispatchSourceCancelHandler

A block to execute when a canceled dispatch source stops executing tasks.


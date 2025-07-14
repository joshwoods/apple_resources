

- DriverKit
- IODataQueueDispatchSource
-  SetEnableWithCompletion 

Instance Method

# SetEnableWithCompletion

Controls the enable state of the interrupt source.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t SetEnableWithCompletion(bool enable, IODispatchSourceCancelHandlerhandler);
```

## Parameters 

`enable`  

A Boolean value that indicates whether to enable the dispatch source. Specify `true` to enable the source or `false` to disable it.

`handler`  

An optional block to execute after this method successfully disables the dispatch source.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Starting and Stopping the Dispatch Source

Cancel

Cancels all callbacks from the dispatch source.


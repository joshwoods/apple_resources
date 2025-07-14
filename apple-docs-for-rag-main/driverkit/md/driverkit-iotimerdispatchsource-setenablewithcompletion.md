

- DriverKit
- IOTimerDispatchSource
-  SetEnableWithCompletion 

Instance Method

# SetEnableWithCompletion

Enables or disables the timer.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t SetEnableWithCompletion(bool enable, IODispatchSourceCancelHandlerhandler);
```

## Parameters 

`enable`  

A Boolean value that indicates whether to enable or disable the timer. Specify true to enable the timer or false to disable it.

`handler`  

An optional block to execute after any pending handlers of a newly disabled timer finish executing.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Starting and Stopping the Timer Source

Cancel

Cancels all callbacks from the event source.


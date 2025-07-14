

- DriverKit
- IODispatchSource
-  SetEnableWithCompletion 

Instance Method

# SetEnableWithCompletion

Enables or disables the dispatch source.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t SetEnableWithCompletion(bool enable, IODispatchSourceCancelHandlerhandler);
```

## Parameters 

`enable`  

A Boolean value that indicates whether to enable or disable the dispatch source. Specify `true` to enable the timer or `false` to disable it.

`handler`  

An optional handler block to execute after disabling the dispatch source. The dispatch source calls your handler after any in-flight callbacks finish.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Subclasses must provide an implementation of this method.

## See Also

### Enabling and Disabling the Source

SetEnable

Enables or disables the delivery of events to your code.


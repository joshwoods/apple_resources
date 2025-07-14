

- DriverKit
- IODispatchSource
-  SetEnable 

Instance Method

# SetEnable

Enables or disables the delivery of events to your code.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t SetEnable(bool enable);
```

## Parameters 

`enable`  

A Boolean value that indicates whether to enable or disable the dispatch source. Specify `true` to enable it or `false` to disable it.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Enabling and Disabling the Source

SetEnableWithCompletion

Enables or disables the dispatch source.


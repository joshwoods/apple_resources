

- Core Foundation
-  CFMachPortInvalidationCallBack 

Type Alias

# CFMachPortInvalidationCallBack

Callback invoked when a CFMachPort object is invalidated.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFMachPortInvalidationCallBack = (CFMachPort?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`port`  

The CFMachPort object that has been invalidated.

`info`  

The `info` member of the CFMachPortContext structure used when creating `port`.

## Discussion

Your callback should free any resources allocated for `port`.

You specify this callback with CFMachPortSetInvalidationCallBack(_:_:).

## See Also

### Callbacks

typealias CFMachPortCallBack

Callback invoked to process a message received on a CFMachPort object.


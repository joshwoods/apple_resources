

- Core Foundation
-  CFMessagePortInvalidationCallBack 

Type Alias

# CFMessagePortInvalidationCallBack

Callback invoked when a CFMessagePort object is invalidated.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFMessagePortInvalidationCallBack = (CFMessagePort?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`ms`  

The message port that has been invalidated.

`info`  

The `info` member of the CFMessagePortContext structure that was used when creating `ms`, if `ms` is a local port; `NULL` if `ms` is a remote port.

## Discussion

Your callback should free any resources allocated for `ms`.

You specify this callback with CFMessagePortSetInvalidationCallBack(_:_:).

## See Also

### Callbacks

typealias CFMessagePortCallBack

Callback invoked to process a message received on a CFMessagePort object.




- Core Foundation
-  CFMessagePortSetInvalidationCallBack(\_:\_:) 

Function

# CFMessagePortSetInvalidationCallBack(\_:\_:)

Sets the callback function invoked when a CFMessagePort object is invalidated.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMessagePortSetInvalidationCallBack(
    _ ms: CFMessagePort!,
    _ callout: CFMessagePortInvalidationCallBack!
)
```

## Parameters 

`ms`  

The message port to examine.

`callout`  

The callback function to invoke when `ms` is invalidated. Pass `NULL` to remove a callback.

## Discussion

If `ms` is already invalid, `callout` is invoked immediately.

## See Also

### Configuring a CFMessagePort Object

func CFMessagePortCreateRunLoopSource(CFAllocator!, CFMessagePort!, CFIndex) -> CFRunLoopSource!

Creates a CFRunLoopSource object for a CFMessagePort object.

func CFMessagePortSetName(CFMessagePort!, CFString!) -> Bool

Sets the name of a local CFMessagePort object.


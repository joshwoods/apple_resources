

- Core Foundation
-  CFMessagePortSetName(\_:\_:) 

Function

# CFMessagePortSetName(\_:\_:)

Sets the name of a local CFMessagePort object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMessagePortSetName(
    _ ms: CFMessagePort!,
    _ newName: CFString!
) -> Bool
```

## Parameters 

`ms`  

The local message port to examine.

`newName`  

The new name for `ms`.

## Return Value

`true` if the name change succeeds, otherwise `false`.

## Discussion

Other threads and processes can connect to a named message port with CFMessagePortCreateRemote(_:_:).

## See Also

### Configuring a CFMessagePort Object

func CFMessagePortCreateRunLoopSource(CFAllocator!, CFMessagePort!, CFIndex) -> CFRunLoopSource!

Creates a CFRunLoopSource object for a CFMessagePort object.

func CFMessagePortSetInvalidationCallBack(CFMessagePort!, CFMessagePortInvalidationCallBack!)

Sets the callback function invoked when a CFMessagePort object is invalidated.


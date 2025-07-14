

- Core Foundation
-  CFMachPortGetContext(\_:\_:) 

Function

# CFMachPortGetContext(\_:\_:)

Returns the context information for a CFMachPort object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMachPortGetContext(
    _ port: CFMachPort!,
    _ context: UnsafeMutablePointer!
)
```

## Parameters 

`port`  

The CFMachPort object to examine.

`context`  

A pointer to the structure into which the context information for `port` is to be copied. The information being returned is usually the same information you passed to CFMachPortCreate(_:_:_:_:) or CFMachPortCreateWithPort(_:_:_:_:_:) when creating `port`. However, if CFMachPortCreateWithPort(_:_:_:_:_:) returned a cached CFMachPort object instead of creating a new object, `context` is filled with information from the original CFMachPort object instead of the information you passed to the function.

## Discussion

The context version number for CFMachPort objects is currently `0`. Before calling this function, you need to initialize the `version` member of `context` to `0`.

## See Also

### Examining a CFMachPort Object

func CFMachPortGetInvalidationCallBack(CFMachPort!) -> CFMachPortInvalidationCallBack!

Returns the invalidation callback function for a CFMachPort object.

func CFMachPortGetPort(CFMachPort!) -> mach_port_t

Returns the native Mach port represented by a CFMachPort object.

func CFMachPortIsValid(CFMachPort!) -> Bool

Returns a Boolean value that indicates whether a CFMachPort object is valid and able to receive messages.


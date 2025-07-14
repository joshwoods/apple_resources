

- Core Foundation
-  CFMachPortGetPort(\_:) 

Function

# CFMachPortGetPort(\_:)

Returns the native Mach port represented by a CFMachPort object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMachPortGetPort(_ port: CFMachPort!) -> mach_port_t
```

## Parameters 

`port`  

The CFMachPort object to examine.

## Return Value

The native Mach port represented by `port`.

## See Also

### Examining a CFMachPort Object

func CFMachPortGetContext(CFMachPort!, UnsafeMutablePointer&lt;CFMachPortContext>!)

Returns the context information for a CFMachPort object.

func CFMachPortGetInvalidationCallBack(CFMachPort!) -> CFMachPortInvalidationCallBack!

Returns the invalidation callback function for a CFMachPort object.

func CFMachPortIsValid(CFMachPort!) -> Bool

Returns a Boolean value that indicates whether a CFMachPort object is valid and able to receive messages.




- Core Foundation
-  CFMachPortIsValid(\_:) 

Function

# CFMachPortIsValid(\_:)

Returns a Boolean value that indicates whether a CFMachPort object is valid and able to receive messages.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMachPortIsValid(_ port: CFMachPort!) -> Bool
```

## Parameters 

`port`  

The CFMachPort object to examine.

## Return Value

`true` if `port` can be used for communication, otherwise `false`.

## See Also

### Examining a CFMachPort Object

func CFMachPortGetContext(CFMachPort!, UnsafeMutablePointer&lt;CFMachPortContext>!)

Returns the context information for a CFMachPort object.

func CFMachPortGetInvalidationCallBack(CFMachPort!) -> CFMachPortInvalidationCallBack!

Returns the invalidation callback function for a CFMachPort object.

func CFMachPortGetPort(CFMachPort!) -> mach_port_t

Returns the native Mach port represented by a CFMachPort object.


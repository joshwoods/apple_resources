

- Core Foundation
-  CFMachPortGetInvalidationCallBack(\_:) 

Function

# CFMachPortGetInvalidationCallBack(\_:)

Returns the invalidation callback function for a CFMachPort object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMachPortGetInvalidationCallBack(_ port: CFMachPort!) -> CFMachPortInvalidationCallBack!
```

## Parameters 

`port`  

The CFMachPort object to examine.

## Return Value

The callback function invoked when `port` is invalidated. `NULL` if no callback has been set with CFMachPortSetInvalidationCallBack(_:_:).

## See Also

### Examining a CFMachPort Object

func CFMachPortGetContext(CFMachPort!, UnsafeMutablePointer&lt;CFMachPortContext>!)

Returns the context information for a CFMachPort object.

func CFMachPortGetPort(CFMachPort!) -> mach_port_t

Returns the native Mach port represented by a CFMachPort object.

func CFMachPortIsValid(CFMachPort!) -> Bool

Returns a Boolean value that indicates whether a CFMachPort object is valid and able to receive messages.




- Core Foundation
-  CFMachPortCallBack 

Type Alias

# CFMachPortCallBack

Callback invoked to process a message received on a CFMachPort object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFMachPortCallBack = (CFMachPort?, UnsafeMutableRawPointer?, CFIndex, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`port`  

The CFMachPort object on which the message `msg` was received.

`msg`  

The Mach message received on `port`. The pointer is to a `mach_msg_header_t` structure.

`size`  

Size of the Mach message `msg`, excluding the message trailer.

`info`  

The `info` member of the CFMachPortContext structure used when creating `port`.

## Discussion

You specify this callback when creating a CFMachPort object with either CFMachPortCreate(_:_:_:_:) or CFMachPortCreateWithPort(_:_:_:_:_:). To receive messages on a CFMachPort object (and have this callback invoked), you must create a run loop source for the port and add it to a run loop.

## See Also

### Callbacks

typealias CFMachPortInvalidationCallBack

Callback invoked when a CFMachPort object is invalidated.


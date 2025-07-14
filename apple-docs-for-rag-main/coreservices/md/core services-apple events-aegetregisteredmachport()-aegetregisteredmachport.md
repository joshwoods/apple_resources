

- Core Services
- Apple Events
-  AEGetRegisteredMachPort() 

Function

# AEGetRegisteredMachPort()

Returns the Mach port (in the form of a `mach_port_t`) that was registered with the bootstrap server for this process.

macOS 10.0+

``` source
func AEGetRegisteredMachPort() -> mach_port_t
```

## Return Value

Returns a Mach message port header.

## Discussion

Apple events in macOS are implemented in terms of Mach messages. If your application links with the Carbon umbrella framework, it includes the HIToolbox framework, which initializes a Mach port and registers it with the run loop for the application. That port is considered public, and is used for sending and receiving Apple events.

Linking with the HIToolbox also requires that the application have a connection to the window server. To facilitate writing server processes that can send and receive Apple events, the Apple Event Manager provides the following functions (in macOS only): `AEGetRegisteredMachPort`, AEDecodeMessage(_:_:_:), AESendMessage(_:_:_:_:), and AEProcessMessage(_:). Daemons and other processes with no user interface can take advantage of these functions, while typical high-level applications will have no need for them.

If your code doesn’t link with the HIToolbox or doesn’t have a run loop, it can call `AEGetRegisteredMachPort` to register a port directly, then listen on that port for Apple events. It can use the other low-level functions to process incoming Apple events on the port and to send Apple events through it.

## See Also

### Working With Lower Level Apple Event Functions

func AEDecodeMessage(UnsafeMutablePointer&lt;mach_msg_header_t>!, UnsafeMutablePointer&lt;AppleEvent>!, UnsafeMutablePointer&lt;AppleEvent>!) -> OSStatus

Decodes a Mach message and converts it into an Apple event and its related reply.

func AESendMessage(UnsafePointer&lt;AppleEvent>!, UnsafeMutablePointer&lt;AppleEvent>!, AESendMode, Int) -> OSStatus

Sends an AppleEvent to a target process without some of the overhead required by `AESend`.

func AEProcessMessage(UnsafeMutablePointer&lt;mach_msg_header_t>!) -> OSStatus

Decodes and dispatches a low level Mach message event to an event handler, including packaging and returning the reply to the sender.


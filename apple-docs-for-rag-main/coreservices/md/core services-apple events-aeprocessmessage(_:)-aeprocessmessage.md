

- Core Services
- Apple Events
-  AEProcessMessage(\_:) 

Function

# AEProcessMessage(\_:)

Decodes and dispatches a low level Mach message event to an event handler, including packaging and returning the reply to the sender.

macOS 10.0+

``` source
func AEProcessMessage(_ header: UnsafeMutablePointer!) -> OSStatus
```

## Parameters 

`header`  

A pointer to the received Mach message that should be processed. The contents of the message header are invalid after calling this method.

## Return Value

A result code. See Result Codes.

## Discussion

The Apple Event Manager provides the following functions (in macOS only) for working with Apple events at a lower level: AEGetRegisteredMachPort(), AEDecodeMessage(_:_:_:), AESendMessage(_:_:_:_:), and `AEProcessMessage`. See the descriptions for those functions for more information on when you might use them.

If your daemon or other code has initialized a Mach port and is listening on it for Apple events and other messages, it can call `AEProcessMessage` to handle any incoming events it identifies as Apple events, while handling other types of events itself. `AEProcessMessage` will dispatch the event to an event handler (by calling `AEDecodeMessage` for you) and package and return the reply to the sender, simplifying handling for your code.

The Apple Event Manager reserves Mach message IDs in the range 0 to 999 for its own use. `AEProcessMessage` returns a `paramErr` result code if the Mach message did not contain an Apple event.

## See Also

### Working With Lower Level Apple Event Functions

func AEGetRegisteredMachPort() -> mach_port_t

Returns the Mach port (in the form of a `mach_port_t`) that was registered with the bootstrap server for this process.

func AEDecodeMessage(UnsafeMutablePointer&lt;mach_msg_header_t>!, UnsafeMutablePointer&lt;AppleEvent>!, UnsafeMutablePointer&lt;AppleEvent>!) -> OSStatus

Decodes a Mach message and converts it into an Apple event and its related reply.

func AESendMessage(UnsafePointer&lt;AppleEvent>!, UnsafeMutablePointer&lt;AppleEvent>!, AESendMode, Int) -> OSStatus

Sends an AppleEvent to a target process without some of the overhead required by `AESend`.


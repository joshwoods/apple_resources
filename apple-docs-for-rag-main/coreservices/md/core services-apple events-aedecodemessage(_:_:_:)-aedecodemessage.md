

- Core Services
- Apple Events
-  AEDecodeMessage(\_:\_:\_:) 

Function

# AEDecodeMessage(\_:\_:\_:)

Decodes a Mach message and converts it into an Apple event and its related reply.

macOS 10.0+

``` source
func AEDecodeMessage(
    _ header: UnsafeMutablePointer!,
    _ event: UnsafeMutablePointer!,
    _ reply: UnsafeMutablePointer!
) -> OSStatus
```

## Parameters 

`header`  

A pointer to a Mach message header for the event to be decoded.

`event`  

A pointer to a null Apple event descriptor (one with descriptor type `typeNull`). On successful completion, contains the decoded Apple event. If the function returns successfully, your application should call the AEDisposeDesc(_:) function to dispose of the resulting descriptor after it has finished using it.

`reply`  

A pointer to a null Apple event descriptor. On successful completion, contains the reply event from the decoded Apple event. To send the reply, you use the following:

## Return Value

A result code. See Result Codes.

## Discussion

The Apple Event Manager provides the following functions (in macOS only) for working with Apple events at a lower level: AEGetRegisteredMachPort(), `AEDecodeMessage`, AESendMessage(_:_:_:_:), and AEProcessMessage(_:). See the descriptions for those functions for more information on when you might use them.

## See Also

### Working With Lower Level Apple Event Functions

func AEGetRegisteredMachPort() -> mach_port_t

Returns the Mach port (in the form of a `mach_port_t`) that was registered with the bootstrap server for this process.

func AESendMessage(UnsafePointer&lt;AppleEvent>!, UnsafeMutablePointer&lt;AppleEvent>!, AESendMode, Int) -> OSStatus

Sends an AppleEvent to a target process without some of the overhead required by `AESend`.

func AEProcessMessage(UnsafeMutablePointer&lt;mach_msg_header_t>!) -> OSStatus

Decodes and dispatches a low level Mach message event to an event handler, including packaging and returning the reply to the sender.


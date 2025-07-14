

- Core MIDI
- MIDISysexSendRequestUMP
-  completionProc 

Instance Property

# completionProc

A function that the system calls after it sends all data for the request, or after the client marks the request as complete.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var completionProc: MIDICompletionProcUMP
```

## See Also

### Configuring and inspecting a request

var destination: MIDIEndpointRef

The endpoint to send the event to.

var words: UnsafeMutablePointer&lt;UInt32>

A pointer to the event to send, which the system advances as it sends the data.

var wordsToSend: UInt32

A counter of the number of words to send.

var complete: DarwinBoolean

A Boolean value that indicates whether the transmission is complete.

typealias MIDICompletionProcUMP

A function the system calls after it completely sends a UMP system-exclusive (SysEx) or SysEx 8-bit event.

var completionRefCon: UnsafeMutableRawPointer?

Data to pass to the completion function.

func MIDIEventPacketSysexBytesForGroup(UnsafePointer&lt;MIDIEventPacket>, UInt8, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>) -> OSStatus

Gets MIDI 1.0 system-exclusive (SysEx) bytes on the indicated group.


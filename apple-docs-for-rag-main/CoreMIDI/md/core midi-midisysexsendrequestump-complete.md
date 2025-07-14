

- Core MIDI
- MIDISysexSendRequestUMP
-  complete 

Instance Property

# complete

A Boolean value that indicates whether the transmission is complete.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var complete: DarwinBoolean
```

## Discussion

Set this value to `true` at any time to abort transmission. The implementation sets the value to `true` after it sends all data.

## See Also

### Configuring and inspecting a request

var destination: MIDIEndpointRef

The endpoint to send the event to.

var words: UnsafeMutablePointer&lt;UInt32>

A pointer to the event to send, which the system advances as it sends the data.

var wordsToSend: UInt32

A counter of the number of words to send.

typealias MIDICompletionProcUMP

A function the system calls after it completely sends a UMP system-exclusive (SysEx) or SysEx 8-bit event.

var completionProc: MIDICompletionProcUMP

A function that the system calls after it sends all data for the request, or after the client marks the request as complete.

var completionRefCon: UnsafeMutableRawPointer?

Data to pass to the completion function.

func MIDIEventPacketSysexBytesForGroup(UnsafePointer&lt;MIDIEventPacket>, UInt8, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>) -> OSStatus

Gets MIDI 1.0 system-exclusive (SysEx) bytes on the indicated group.


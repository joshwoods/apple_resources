

- Core MIDI
- MIDISysexSendRequest
-  completionProc 

Instance Property

# completionProc

A function that the system calls after it sends all bytes for the request, or after the client marks the request as complete.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var completionProc: MIDICompletionProc
```

## See Also

### Configuring a request

var destination: MIDIEndpointRef

The endpoint to send the event to.

var data: UnsafePointer&lt;UInt8>

The request’s data.

var bytesToSend: UInt32

The number of bytes to send.

var complete: DarwinBoolean

A Boolean value that indicates whether the transmission is complete.

typealias MIDICompletionProc

A function the system calls after it completely sends a system-exclusive (SysEx) event.

var completionRefCon: UnsafeMutableRawPointer?

Data to pass to the completion function.

var reserved: (UInt8, UInt8, UInt8)

A field that’s reserved for future use.


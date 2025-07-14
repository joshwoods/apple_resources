

- Core MIDI
- MIDISysexSendRequest
-  data 

Instance Property

# data

The request’s data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var data: UnsafePointer
```

## Discussion

Initially, the value is a pointer to the System Exclusive (SysEx) event to send. MIDISendSysex(_:) advances this pointer as it sends bytes.

## See Also

### Configuring a request

var destination: MIDIEndpointRef

The endpoint to send the event to.

var bytesToSend: UInt32

The number of bytes to send.

var complete: DarwinBoolean

A Boolean value that indicates whether the transmission is complete.

typealias MIDICompletionProc

A function the system calls after it completely sends a system-exclusive (SysEx) event.

var completionProc: MIDICompletionProc

A function that the system calls after it sends all bytes for the request, or after the client marks the request as complete.

var completionRefCon: UnsafeMutableRawPointer?

Data to pass to the completion function.

var reserved: (UInt8, UInt8, UInt8)

A field that’s reserved for future use.


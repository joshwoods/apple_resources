

- Core MIDI
-  MIDISysexSendRequest 

Structure

# MIDISysexSendRequest

A request to asynchronously send a single system-exclusive (SysEx) event to a destination.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MIDISysexSendRequest
```

## Topics

### Creating a request

init(destination: MIDIEndpointRef, data: UnsafePointer&lt;UInt8>, bytesToSend: UInt32, complete: DarwinBoolean, reserved: (UInt8, UInt8, UInt8), completionProc: MIDICompletionProc, completionRefCon: UnsafeMutableRawPointer?)

Creates a new single system-exclusive (SysEx) event request.

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

var completionProc: MIDICompletionProc

A function that the system calls after it sends all bytes for the request, or after the client marks the request as complete.

var completionRefCon: UnsafeMutableRawPointer?

Data to pass to the completion function.

var reserved: (UInt8, UInt8, UInt8)

A field that’s reserved for future use.

### Sending a request

func MIDISendSysex(UnsafeMutablePointer&lt;MIDISysexSendRequest>) -> OSStatus

Asynchronously sends a single system-exclusive (SysEx) event.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### I/O management

struct MIDISysexSendRequestUMP

A request to asynchronously send a single universal MIDI packet (UMP) system-exclusive (SysEx) event to a destination.

func MIDIFlushOutput(MIDIEndpointRef) -> OSStatus

Cancels all pending events that were previously scheduled to send.

func MIDIRestart() -> OSStatus

Stops and restarts MIDI I/O.

struct MIDIIOErrorNotification

A general I/O error notification.


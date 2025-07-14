

- Core MIDI
-  MIDISysexSendRequestUMP 

Structure

# MIDISysexSendRequestUMP

A request to asynchronously send a single universal MIDI packet (UMP) system-exclusive (SysEx) event to a destination.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MIDISysexSendRequestUMP
```

## Topics

### Creating a request

init(destination: MIDIEndpointRef, words: UnsafeMutablePointer&lt;UInt32>, wordsToSend: UInt32, complete: DarwinBoolean, completionProc: MIDICompletionProcUMP, completionRefCon: UnsafeMutableRawPointer?)

Creates a new single universal MIDI packet (UMP) system-exclusive (SysEx) event request.

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

var completionProc: MIDICompletionProcUMP

A function that the system calls after it sends all data for the request, or after the client marks the request as complete.

var completionRefCon: UnsafeMutableRawPointer?

Data to pass to the completion function.

func MIDIEventPacketSysexBytesForGroup(UnsafePointer&lt;MIDIEventPacket>, UInt8, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>) -> OSStatus

Gets MIDI 1.0 system-exclusive (SysEx) bytes on the indicated group.

### Sending a request

func MIDISendUMPSysex(UnsafeMutablePointer&lt;MIDISysexSendRequestUMP>) -> OSStatus

Asynchronously sends a single universal MIDI packet (UMP) system-exclusive (SysEx) event.

func MIDISendUMPSysex8(UnsafeMutablePointer&lt;MIDISysexSendRequestUMP>) -> OSStatus

Asynchronously sends a single universal MIDI packet (UMP) system-exclusive (SysEx) event with an 8-bit message.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### I/O management

struct MIDISysexSendRequest

A request to asynchronously send a single system-exclusive (SysEx) event to a destination.

func MIDIFlushOutput(MIDIEndpointRef) -> OSStatus

Cancels all pending events that were previously scheduled to send.

func MIDIRestart() -> OSStatus

Stops and restarts MIDI I/O.

struct MIDIIOErrorNotification

A general I/O error notification.


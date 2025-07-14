

- Core MIDI
-  MIDIRestart() 

Function

# MIDIRestart()

Stops and restarts MIDI I/O.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.1+visionOS 1.0+

``` source
func MIDIRestart() -> OSStatus
```

## Return Value

An `OSStatus` result code.

## Discussion

Call this function to force Core MIDI to ask its drivers to rescan for hardware.

## See Also

### I/O management

struct MIDISysexSendRequest

A request to asynchronously send a single system-exclusive (SysEx) event to a destination.

struct MIDISysexSendRequestUMP

A request to asynchronously send a single universal MIDI packet (UMP) system-exclusive (SysEx) event to a destination.

func MIDIFlushOutput(MIDIEndpointRef) -> OSStatus

Cancels all pending events that were previously scheduled to send.

struct MIDIIOErrorNotification

A general I/O error notification.


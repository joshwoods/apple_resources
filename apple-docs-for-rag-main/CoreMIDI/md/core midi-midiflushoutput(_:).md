

- Core MIDI
-  MIDIFlushOutput(\_:) 

Function

# MIDIFlushOutput(\_:)

Cancels all pending events that were previously scheduled to send.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.1+visionOS 1.0+

``` source
func MIDIFlushOutput(_ dest: MIDIEndpointRef) -> OSStatus
```

## Parameters 

`dest`  

The destination with pending events to cancel. If nil, the operation applies to all destinations.

## Return Value

An `OSStatus` result code.

## See Also

### I/O management

struct MIDISysexSendRequest

A request to asynchronously send a single system-exclusive (SysEx) event to a destination.

struct MIDISysexSendRequestUMP

A request to asynchronously send a single universal MIDI packet (UMP) system-exclusive (SysEx) event to a destination.

func MIDIRestart() -> OSStatus

Stops and restarts MIDI I/O.

struct MIDIIOErrorNotification

A general I/O error notification.


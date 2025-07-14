

- Core MIDI
-  MIDISendUMPSysex8(\_:) 

Function

# MIDISendUMPSysex8(\_:)

Asynchronously sends a single universal MIDI packet (UMP) system-exclusive (SysEx) event with an 8-bit message.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
func MIDISendUMPSysex8(_ umpRequest: UnsafeMutablePointer) -> OSStatus
```

## Parameters 

`umpRequest`  

Contains the destination and a pointer to the MIDI data to send.

## Return Value

An `OSStatus` result code.

## Discussion

The request’s data needs to point to a single MIDI SysEx 8-bit message, or portion thereof.

## See Also

### Sending a request

func MIDISendUMPSysex(UnsafeMutablePointer&lt;MIDISysexSendRequestUMP>) -> OSStatus

Asynchronously sends a single universal MIDI packet (UMP) system-exclusive (SysEx) event.


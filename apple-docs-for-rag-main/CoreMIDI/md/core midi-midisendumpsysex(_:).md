

- Core MIDI
-  MIDISendUMPSysex(\_:) 

Function

# MIDISendUMPSysex(\_:)

Asynchronously sends a single universal MIDI packet (UMP) system-exclusive (SysEx) event.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
func MIDISendUMPSysex(_ umpRequest: UnsafeMutablePointer) -> OSStatus
```

## Parameters 

`umpRequest`  

Contains the destination and a pointer to the MIDI data to send.

## Return Value

An `OSStatus` result code.

## Discussion

The request’s words needs to point to a single MIDI SysEx message, or portion thereof.

## See Also

### Sending a request

func MIDISendUMPSysex8(UnsafeMutablePointer&lt;MIDISysexSendRequestUMP>) -> OSStatus

Asynchronously sends a single universal MIDI packet (UMP) system-exclusive (SysEx) event with an 8-bit message.


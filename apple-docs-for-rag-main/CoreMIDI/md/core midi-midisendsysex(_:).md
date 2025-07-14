

- Core MIDI
-  MIDISendSysex(\_:) 

Function

# MIDISendSysex(\_:)

Asynchronously sends a single system-exclusive (SysEx) event.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDISendSysex(_ request: UnsafeMutablePointer) -> OSStatus
```

## Parameters 

`request`  

Contains the destination and a pointer to the MIDI data to send.

## Return Value

An `OSStatus` result code.


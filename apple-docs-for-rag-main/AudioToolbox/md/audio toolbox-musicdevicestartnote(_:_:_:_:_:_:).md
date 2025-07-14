

- Audio Toolbox
-  MusicDeviceStartNote(\_:\_:\_:\_:\_:\_:) 

Function

# MusicDeviceStartNote(\_:\_:\_:\_:\_:\_:)

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func MusicDeviceStartNote(
    _ inUnit: MusicDeviceComponent,
    _ inInstrument: MusicDeviceInstrumentID,
    _ inGroupID: MusicDeviceGroupID,
    _ outNoteInstanceID: UnsafeMutablePointer,
    _ inOffsetSampleFrame: UInt32,
    _ inParams: UnsafePointer
) -> OSStatus
```

## See Also

### Interacting with Music Devices

func MusicDeviceMIDIEvent(MusicDeviceComponent, UInt32, UInt32, UInt32, UInt32) -> OSStatus

func MusicDeviceMIDIEventList(MusicDeviceComponent, UInt32, UnsafePointer&lt;MIDIEventList>) -> OSStatus

func MusicDeviceStopNote(MusicDeviceComponent, MusicDeviceGroupID, NoteInstanceID, UInt32) -> OSStatus

func MusicDeviceSysEx(MusicDeviceComponent, UnsafePointer&lt;UInt8>, UInt32) -> OSStatus

typealias MusicDeviceComponent

typealias MusicDeviceGroupID

typealias MusicDeviceInstrumentID

typealias MusicDeviceMIDIEventProc

typealias MusicDeviceStartNoteProc

typealias MusicDeviceStopNoteProc

typealias MusicDeviceSysExProc




- Audio Toolbox
-  MusicDeviceMIDIEvent(\_:\_:\_:\_:\_:) 

Function

# MusicDeviceMIDIEvent(\_:\_:\_:\_:\_:)

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func MusicDeviceMIDIEvent(
    _ inUnit: MusicDeviceComponent,
    _ inStatus: UInt32,
    _ inData1: UInt32,
    _ inData2: UInt32,
    _ inOffsetSampleFrame: UInt32
) -> OSStatus
```

## See Also

### Interacting with Music Devices

func MusicDeviceMIDIEventList(MusicDeviceComponent, UInt32, UnsafePointer&lt;MIDIEventList>) -> OSStatus

func MusicDeviceStartNote(MusicDeviceComponent, MusicDeviceInstrumentID, MusicDeviceGroupID, UnsafeMutablePointer&lt;NoteInstanceID>, UInt32, UnsafePointer&lt;MusicDeviceNoteParams>) -> OSStatus

func MusicDeviceStopNote(MusicDeviceComponent, MusicDeviceGroupID, NoteInstanceID, UInt32) -> OSStatus

func MusicDeviceSysEx(MusicDeviceComponent, UnsafePointer&lt;UInt8>, UInt32) -> OSStatus

typealias MusicDeviceComponent

typealias MusicDeviceGroupID

typealias MusicDeviceInstrumentID

typealias MusicDeviceMIDIEventProc

typealias MusicDeviceStartNoteProc

typealias MusicDeviceStopNoteProc

typealias MusicDeviceSysExProc


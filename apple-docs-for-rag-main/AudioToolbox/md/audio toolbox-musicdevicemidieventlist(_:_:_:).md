

- Audio Toolbox
-  MusicDeviceMIDIEventList(\_:\_:\_:) 

Function

# MusicDeviceMIDIEventList(\_:\_:\_:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func MusicDeviceMIDIEventList(
    _ inUnit: MusicDeviceComponent,
    _ inOffsetSampleFrame: UInt32,
    _ evtList: UnsafePointer
) -> OSStatus
```

## See Also

### Interacting with Music Devices

func MusicDeviceMIDIEvent(MusicDeviceComponent, UInt32, UInt32, UInt32, UInt32) -> OSStatus

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


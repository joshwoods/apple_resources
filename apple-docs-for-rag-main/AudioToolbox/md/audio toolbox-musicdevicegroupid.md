

- Audio Toolbox
-  MusicDeviceGroupID 

Type Alias

# MusicDeviceGroupID

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias MusicDeviceGroupID = UInt32
```

## See Also

### Interacting with Music Devices

func MusicDeviceMIDIEvent(MusicDeviceComponent, UInt32, UInt32, UInt32, UInt32) -> OSStatus

func MusicDeviceMIDIEventList(MusicDeviceComponent, UInt32, UnsafePointer&lt;MIDIEventList>) -> OSStatus

func MusicDeviceStartNote(MusicDeviceComponent, MusicDeviceInstrumentID, MusicDeviceGroupID, UnsafeMutablePointer&lt;NoteInstanceID>, UInt32, UnsafePointer&lt;MusicDeviceNoteParams>) -> OSStatus

func MusicDeviceStopNote(MusicDeviceComponent, MusicDeviceGroupID, NoteInstanceID, UInt32) -> OSStatus

func MusicDeviceSysEx(MusicDeviceComponent, UnsafePointer&lt;UInt8>, UInt32) -> OSStatus

typealias MusicDeviceComponent

typealias MusicDeviceInstrumentID

typealias MusicDeviceMIDIEventProc

typealias MusicDeviceStartNoteProc

typealias MusicDeviceStopNoteProc

typealias MusicDeviceSysExProc




- Audio Toolbox
-  MusicDeviceInstrumentID 

Type Alias

# MusicDeviceInstrumentID

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias MusicDeviceInstrumentID = UInt32
```

## See Also

### Interacting with Music Devices

func MusicDeviceMIDIEvent(MusicDeviceComponent, UInt32, UInt32, UInt32, UInt32) -> OSStatus

func MusicDeviceMIDIEventList(MusicDeviceComponent, UInt32, UnsafePointer&lt;MIDIEventList>) -> OSStatus

func MusicDeviceStartNote(MusicDeviceComponent, MusicDeviceInstrumentID, MusicDeviceGroupID, UnsafeMutablePointer&lt;NoteInstanceID>, UInt32, UnsafePointer&lt;MusicDeviceNoteParams>) -> OSStatus

func MusicDeviceStopNote(MusicDeviceComponent, MusicDeviceGroupID, NoteInstanceID, UInt32) -> OSStatus

func MusicDeviceSysEx(MusicDeviceComponent, UnsafePointer&lt;UInt8>, UInt32) -> OSStatus

typealias MusicDeviceComponent

typealias MusicDeviceGroupID

typealias MusicDeviceMIDIEventProc

typealias MusicDeviceStartNoteProc

typealias MusicDeviceStopNoteProc

typealias MusicDeviceSysExProc


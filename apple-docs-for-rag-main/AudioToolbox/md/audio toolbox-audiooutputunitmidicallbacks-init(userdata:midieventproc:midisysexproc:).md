

- Audio Toolbox
- AudioOutputUnitMIDICallbacks
-  init(userData:MIDIEventProc:MIDISysExProc:) 

Initializer

# init(userData:MIDIEventProc:MIDISysExProc:)

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
init(
    userData: UnsafeMutableRawPointer?,
    MIDIEventProc: (UnsafeMutableRawPointer?, UInt32, UInt32, UInt32, UInt32) -> Void,
    MIDISysExProc: (UnsafeMutableRawPointer?, UnsafePointer, UInt32) -> Void
)
```


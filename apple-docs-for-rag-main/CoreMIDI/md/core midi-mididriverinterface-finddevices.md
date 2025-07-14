

- Core MIDI
- MIDIDriverInterface
-  FindDevices 

Instance Property

# FindDevices

Finds the available devices.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var FindDevices: (MIDIDriverRef, MIDIDeviceListRef) -> OSStatus
```

## Discussion

Don’t hold strong references to the created devices and entities.

## See Also

### Properties

var Start: (MIDIDriverRef, MIDIDeviceListRef) -> OSStatus

Starts MIDI I/O.

var Stop: (MIDIDriverRef) -> OSStatus

Stops MIDI I/O.

var Configure: (MIDIDriverRef, MIDIDeviceRef) -> OSStatus

The system doesn’t currently use this method.

var Send: (MIDIDriverRef, UnsafePointer&lt;MIDIPacketList>, UnsafeMutableRawPointer, UnsafeMutableRawPointer) -> OSStatus

Sends a MIDI packet list to the specified destination endpoints.

var EnableSource: (MIDIDriverRef, MIDIEndpointRef, DarwinBoolean) -> OSStatus

Tells the driver whether input from a particular source has listeners.

var Flush: (MIDIDriverRef, MIDIEndpointRef, UnsafeMutableRawPointer?, UnsafeMutableRawPointer?) -> OSStatus

Unschedules all pending output to the specified destination.

var Monitor: (MIDIDriverRef, MIDIEndpointRef, UnsafePointer&lt;MIDIPacketList>) -> OSStatus

Enables monitoring of MIDI packet lists by the specified driver.

var MonitorEvents: (MIDIDriverRef, MIDIEndpointRef, UnsafePointer&lt;MIDIEventList>) -> OSStatus

Enables monitoring of MIDI event lists by the specified driver.

var SendPackets: (MIDIDriverRef, UnsafePointer&lt;MIDIEventList>, UnsafeMutableRawPointer, UnsafeMutableRawPointer) -> OSStatus

Sends a MIDI event list to the specified destination endpoints.

var AddRef: (UnsafeMutableRawPointer) -> ULONG

var QueryInterface: (UnsafeMutableRawPointer, REFIID, UnsafeMutablePointer&lt;LPVOID?>?) -> HRESULT

var Release: (UnsafeMutableRawPointer) -> ULONG


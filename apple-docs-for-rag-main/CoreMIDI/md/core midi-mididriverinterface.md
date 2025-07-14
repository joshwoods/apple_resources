

- Core MIDI
-  MIDIDriverInterface 

Structure

# MIDIDriverInterface

The interface to a MIDI driver.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MIDIDriverInterface
```

## Topics

### Properties

var FindDevices: (MIDIDriverRef, MIDIDeviceListRef) -> OSStatus

Finds the available devices.

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

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Inspecting a Driver

func MIDIGetDriverDeviceList(MIDIDriverRef) -> MIDIDeviceListRef

Returns the list of driver-created devices in the current MIDI setup.

func MIDIDriverEnableMonitoring(MIDIDriverRef, Bool) -> OSStatus

Enables monitoring of all outgoing MIDI packets.

func MIDIGetDriverIORunLoop() -> Unmanaged&lt;CFRunLoop>

Returns the server’s driver I/O thread.

let kMIDIDriverPropertyUsesSerial: CFString

A value that indicates whether the driver uses serial ports and is eligible to have serial ports assigned to it.

typealias MIDIDriverRef

A MIDI driver object.


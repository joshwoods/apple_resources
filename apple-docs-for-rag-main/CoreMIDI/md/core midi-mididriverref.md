

- Core MIDI
-  MIDIDriverRef 

Type Alias

# MIDIDriverRef

A MIDI driver object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias MIDIDriverRef = UnsafeMutablePointer>
```

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

struct MIDIDriverInterface

The interface to a MIDI driver.


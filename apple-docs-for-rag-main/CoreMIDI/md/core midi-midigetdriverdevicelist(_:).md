

- Core MIDI
-  MIDIGetDriverDeviceList(\_:) 

Function

# MIDIGetDriverDeviceList(\_:)

Returns the list of driver-created devices in the current MIDI setup.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.1+visionOS 1.0+

``` source
func MIDIGetDriverDeviceList(_ driver: MIDIDriverRef) -> MIDIDeviceListRef
```

## Parameters 

`driver`  

The driver for which you return devices.

## Return Value

The requested device list.

## Discussion

Dispose this list when you’re finished working with it by calling MIDIDeviceListDispose(_:).

## See Also

### Inspecting a Driver

func MIDIDriverEnableMonitoring(MIDIDriverRef, Bool) -> OSStatus

Enables monitoring of all outgoing MIDI packets.

func MIDIGetDriverIORunLoop() -> Unmanaged&lt;CFRunLoop>

Returns the server’s driver I/O thread.

let kMIDIDriverPropertyUsesSerial: CFString

A value that indicates whether the driver uses serial ports and is eligible to have serial ports assigned to it.

struct MIDIDriverInterface

The interface to a MIDI driver.

typealias MIDIDriverRef

A MIDI driver object.


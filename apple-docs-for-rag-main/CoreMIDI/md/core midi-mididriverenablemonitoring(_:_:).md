

- Core MIDI
-  MIDIDriverEnableMonitoring(\_:\_:) 

Function

# MIDIDriverEnableMonitoring(\_:\_:)

Enables monitoring of all outgoing MIDI packets.

macOS 10.1+

``` source
func MIDIDriverEnableMonitoring(
    _ driver: MIDIDriverRef,
    _ enabled: Bool
) -> OSStatus
```

## Parameters 

`driver`  

The driver for which to enable monitoring.

`enabled`  

A Boolean value that indicates whether to enable monitoring.

## Return Value

An `OSStatus` result code.

## Discussion

Some specialized drivers, like a MIDI monitor display, can intercept and inspect all outgoing MIDI messages. Enablng monitoring causes the system to call the Monitor function with the outgoing MIDI packets for all destinations in the system. The Monitor function can’t rely on the MIDI events arriving in order, due to the MIDI server’s schedule-ahead facilities.

## See Also

### Inspecting a Driver

func MIDIGetDriverDeviceList(MIDIDriverRef) -> MIDIDeviceListRef

Returns the list of driver-created devices in the current MIDI setup.

func MIDIGetDriverIORunLoop() -> Unmanaged&lt;CFRunLoop>

Returns the server’s driver I/O thread.

let kMIDIDriverPropertyUsesSerial: CFString

A value that indicates whether the driver uses serial ports and is eligible to have serial ports assigned to it.

struct MIDIDriverInterface

The interface to a MIDI driver.

typealias MIDIDriverRef

A MIDI driver object.


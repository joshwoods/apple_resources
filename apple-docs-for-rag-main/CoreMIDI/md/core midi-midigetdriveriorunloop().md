

- Core MIDI
-  MIDIGetDriverIORunLoop() 

Function

# MIDIGetDriverIORunLoop()

Returns the server’s driver I/O thread.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIGetDriverIORunLoop() -> Unmanaged
```

## Return Value

The CFRunLoop of the server’s driver I/O thread.

## Discussion

Drivers typically need to receive asynchronous I/O completion callbacks on a high-priority thread. So that the system can efficiently manage resources, the MIDI server provides a thread which drivers may use. This is a realtime-priority thread that drivers shouldn’t use for anything other than I/O.

## See Also

### Inspecting a Driver

func MIDIGetDriverDeviceList(MIDIDriverRef) -> MIDIDeviceListRef

Returns the list of driver-created devices in the current MIDI setup.

func MIDIDriverEnableMonitoring(MIDIDriverRef, Bool) -> OSStatus

Enables monitoring of all outgoing MIDI packets.

let kMIDIDriverPropertyUsesSerial: CFString

A value that indicates whether the driver uses serial ports and is eligible to have serial ports assigned to it.

struct MIDIDriverInterface

The interface to a MIDI driver.

typealias MIDIDriverRef

A MIDI driver object.


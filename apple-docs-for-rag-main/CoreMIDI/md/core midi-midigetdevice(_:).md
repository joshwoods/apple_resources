

- Core MIDI
-  MIDIGetDevice(\_:) 

Function

# MIDIGetDevice(\_:)

Returns a device from the system.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIGetDevice(_ deviceIndex0: Int) -> MIDIDeviceRef
```

## Parameters 

`deviceIndex0`  

The index of the device to retrieve.

## Return Value

A reference to a device, or `NULL` if an error occurred.

## Discussion

Call this function to enumerate the devices in the system. To enumerate the entities in the system, walk through the devices and then walk through the device’s entities. When you iterate through the devices and entities in the system, you don’t visit virtual sources and destinations created by other clients.

A device iteration returns devices that are *offline* (they were present in the past but aren’t currently available), while iterations through the system’s sources and destinations don’t include the endpoints of offline devices. Instead, clients typically use MIDIGetNumberOfSources(), MIDIGetSource(_:), MIDIGetNumberOfDestinations() and MIDIGetDestination(_:).

## See Also

### Device lookup

func MIDIGetNumberOfDevices() -> Int

Returns the number of devices in the system.

func MIDIGetNumberOfExternalDevices() -> Int

Returns the number of external MIDI devices in the system.

func MIDIGetExternalDevice(Int) -> MIDIDeviceRef

Returns one of the external devices in the system.

func MIDIDeviceGetNumberOfEntities(MIDIDeviceRef) -> Int

Returns the number of entities in a device.

func MIDIDeviceGetEntity(MIDIDeviceRef, Int) -> MIDIEntityRef

Returns the device’s entity at a specific index.

typealias MIDIDeviceRef

A MIDI device that contains entities.


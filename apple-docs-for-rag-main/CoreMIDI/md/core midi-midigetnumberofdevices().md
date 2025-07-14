

- Core MIDI
-  MIDIGetNumberOfDevices() 

Function

# MIDIGetNumberOfDevices()

Returns the number of devices in the system.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIGetNumberOfDevices() -> Int
```

## Return Value

The number of devices in the system, or 0 if an error occurred.

## See Also

### Device lookup

func MIDIGetDevice(Int) -> MIDIDeviceRef

Returns a device from the system.

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


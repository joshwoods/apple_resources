

- Core MIDI
-  MIDIGetNumberOfExternalDevices() 

Function

# MIDIGetNumberOfExternalDevices()

Returns the number of external MIDI devices in the system.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.1+visionOS 1.0+

``` source
func MIDIGetNumberOfExternalDevices() -> Int
```

## Return Value

The number of external devices in the system, or 0 if an error occurred.

## Discussion

External MIDI devices connect to driver endpoints using a standard MIDI cable. Their presence is optional only when a UI (such as Audio MIDI Setup) adds them.

## See Also

### Device lookup

func MIDIGetNumberOfDevices() -> Int

Returns the number of devices in the system.

func MIDIGetDevice(Int) -> MIDIDeviceRef

Returns a device from the system.

func MIDIGetExternalDevice(Int) -> MIDIDeviceRef

Returns one of the external devices in the system.

func MIDIDeviceGetNumberOfEntities(MIDIDeviceRef) -> Int

Returns the number of entities in a device.

func MIDIDeviceGetEntity(MIDIDeviceRef, Int) -> MIDIEntityRef

Returns the device’s entity at a specific index.

typealias MIDIDeviceRef

A MIDI device that contains entities.


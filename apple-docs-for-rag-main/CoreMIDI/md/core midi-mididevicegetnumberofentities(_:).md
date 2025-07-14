

- Core MIDI
-  MIDIDeviceGetNumberOfEntities(\_:) 

Function

# MIDIDeviceGetNumberOfEntities(\_:)

Returns the number of entities in a device.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIDeviceGetNumberOfEntities(_ device: MIDIDeviceRef) -> Int
```

## Parameters 

`device`  

The device to query.

## Return Value

The number of entities the device contains, or 0 if an error occurred.

## See Also

### Device lookup

func MIDIGetNumberOfDevices() -> Int

Returns the number of devices in the system.

func MIDIGetDevice(Int) -> MIDIDeviceRef

Returns a device from the system.

func MIDIGetNumberOfExternalDevices() -> Int

Returns the number of external MIDI devices in the system.

func MIDIGetExternalDevice(Int) -> MIDIDeviceRef

Returns one of the external devices in the system.

func MIDIDeviceGetEntity(MIDIDeviceRef, Int) -> MIDIEntityRef

Returns the device’s entity at a specific index.

typealias MIDIDeviceRef

A MIDI device that contains entities.


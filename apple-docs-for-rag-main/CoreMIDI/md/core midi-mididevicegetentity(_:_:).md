

- Core MIDI
-  MIDIDeviceGetEntity(\_:\_:) 

Function

# MIDIDeviceGetEntity(\_:\_:)

Returns the device’s entity at a specific index.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIDeviceGetEntity(
    _ device: MIDIDeviceRef,
    _ entityIndex0: Int
) -> MIDIEntityRef
```

## Parameters 

`device`  

The device to query.

`entityIndex0`  

The entity index.

## Return Value

An entity reference, or `NULL` if an error occurred.

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

func MIDIDeviceGetNumberOfEntities(MIDIDeviceRef) -> Int

Returns the number of entities in a device.

typealias MIDIDeviceRef

A MIDI device that contains entities.


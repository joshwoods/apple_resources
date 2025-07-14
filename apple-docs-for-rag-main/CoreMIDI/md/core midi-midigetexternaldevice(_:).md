

- Core MIDI
-  MIDIGetExternalDevice(\_:) 

Function

# MIDIGetExternalDevice(\_:)

Returns one of the external devices in the system.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.1+visionOS 1.0+

``` source
func MIDIGetExternalDevice(_ deviceIndex0: Int) -> MIDIDeviceRef
```

## Parameters 

`deviceIndex0`  

The index of the device to return.

## Return Value

A reference to a device, or `NULL` if an error occurred.

## Discussion

Call this function to enumerate the external devices in the system.

## See Also

### Device lookup

func MIDIGetNumberOfDevices() -> Int

Returns the number of devices in the system.

func MIDIGetDevice(Int) -> MIDIDeviceRef

Returns a device from the system.

func MIDIGetNumberOfExternalDevices() -> Int

Returns the number of external MIDI devices in the system.

func MIDIDeviceGetNumberOfEntities(MIDIDeviceRef) -> Int

Returns the number of entities in a device.

func MIDIDeviceGetEntity(MIDIDeviceRef, Int) -> MIDIEntityRef

Returns the device’s entity at a specific index.

typealias MIDIDeviceRef

A MIDI device that contains entities.


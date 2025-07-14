

- Core MIDI
-  MIDIDeviceRemoveEntity(\_:\_:) 

Function

# MIDIDeviceRemoveEntity(\_:\_:)

Removes an entity from a device.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.1+visionOS 1.0+

``` source
func MIDIDeviceRemoveEntity(
    _ device: MIDIDeviceRef,
    _ entity: MIDIEntityRef
) -> OSStatus
```

## Parameters 

`device`  

The device to update.

`entity`  

The entity to remove.

## Return Value

An `OSStatus` result code.

## Discussion

Drivers call this function to remove one of a device’s entities.

## See Also

### Managing Entities

func MIDIDeviceNewEntity(MIDIDeviceRef, CFString, MIDIProtocolID, Bool, Int, Int, UnsafeMutablePointer&lt;MIDIEntityRef>) -> OSStatus

Adds a new entity to a device.

func MIDIEntityAddOrRemoveEndpoints(MIDIEntityRef, Int, Int) -> OSStatus

Adds or removes an entity’s endpoints.


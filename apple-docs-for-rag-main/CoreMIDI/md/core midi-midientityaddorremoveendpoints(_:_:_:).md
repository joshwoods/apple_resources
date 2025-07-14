

- Core MIDI
-  MIDIEntityAddOrRemoveEndpoints(\_:\_:\_:) 

Function

# MIDIEntityAddOrRemoveEndpoints(\_:\_:\_:)

Adds or removes an entity’s endpoints.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.2+visionOS 1.0+

``` source
func MIDIEntityAddOrRemoveEndpoints(
    _ entity: MIDIEntityRef,
    _ numSourceEndpoints: Int,
    _ numDestinationEndpoints: Int
) -> OSStatus
```

## Parameters 

`entity`  

The entity to update.

`numSourceEndpoints`  

The number of source endpoints.

`numDestinationEndpoints`  

The number of destination endpoints.

## Return Value

An `OSStatus` result code.

## Discussion

Drivers and configuration editors may call this function to add to or remove an entity’s endpoints. The MIDIProtocolID of new endpoints is initially the same as that of the entity.

## See Also

### Managing Entities

func MIDIDeviceNewEntity(MIDIDeviceRef, CFString, MIDIProtocolID, Bool, Int, Int, UnsafeMutablePointer&lt;MIDIEntityRef>) -> OSStatus

Adds a new entity to a device.

func MIDIDeviceRemoveEntity(MIDIDeviceRef, MIDIEntityRef) -> OSStatus

Removes an entity from a device.




- Core MIDI
-  MIDIEntityGetDevice(\_:\_:) 

Function

# MIDIEntityGetDevice(\_:\_:)

Returns an entity’s device.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.2+visionOS 1.0+

``` source
func MIDIEntityGetDevice(
    _ inEntity: MIDIEntityRef,
    _ outDevice: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`inEntity`  

The entity to query.

`outDevice`  

On successful return, the entity’s owning device.

## Return Value

An `OSStatus` result code.

## See Also

### Entity lookup

func MIDIEntityGetNumberOfSources(MIDIEntityRef) -> Int

Returns the number of sources in an entity.

func MIDIEntityGetSource(MIDIEntityRef, Int) -> MIDIEndpointRef

Returns one of an entity’s sources.

func MIDIEntityGetNumberOfDestinations(MIDIEntityRef) -> Int

Returns the number of destinations in an entity.

func MIDIEntityGetDestination(MIDIEntityRef, Int) -> MIDIEndpointRef

Returns one of an entity’s destinations.

typealias MIDIEntityRef

An entity that a device owns and that contains endpoints.




- Core MIDI
-  MIDIEntityGetNumberOfDestinations(\_:) 

Function

# MIDIEntityGetNumberOfDestinations(\_:)

Returns the number of destinations in an entity.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIEntityGetNumberOfDestinations(_ entity: MIDIEntityRef) -> Int
```

## Parameters 

`entity`  

The entity to query.

## Return Value

The number of destinations the entity contains, or 0 if an error occurred.

## See Also

### Entity lookup

func MIDIEntityGetDevice(MIDIEntityRef, UnsafeMutablePointer&lt;MIDIDeviceRef>?) -> OSStatus

Returns an entity’s device.

func MIDIEntityGetNumberOfSources(MIDIEntityRef) -> Int

Returns the number of sources in an entity.

func MIDIEntityGetSource(MIDIEntityRef, Int) -> MIDIEndpointRef

Returns one of an entity’s sources.

func MIDIEntityGetDestination(MIDIEntityRef, Int) -> MIDIEndpointRef

Returns one of an entity’s destinations.

typealias MIDIEntityRef

An entity that a device owns and that contains endpoints.


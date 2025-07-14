

- Core MIDI
-  MIDIEntityGetNumberOfSources(\_:) 

Function

# MIDIEntityGetNumberOfSources(\_:)

Returns the number of sources in an entity.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIEntityGetNumberOfSources(_ entity: MIDIEntityRef) -> Int
```

## Parameters 

`entity`  

The entity to query.

## Return Value

The number of sources the entity contains, or 0 if an error occurred.

## See Also

### Entity lookup

func MIDIEntityGetDevice(MIDIEntityRef, UnsafeMutablePointer&lt;MIDIDeviceRef>?) -> OSStatus

Returns an entity’s device.

func MIDIEntityGetSource(MIDIEntityRef, Int) -> MIDIEndpointRef

Returns one of an entity’s sources.

func MIDIEntityGetNumberOfDestinations(MIDIEntityRef) -> Int

Returns the number of destinations in an entity.

func MIDIEntityGetDestination(MIDIEntityRef, Int) -> MIDIEndpointRef

Returns one of an entity’s destinations.

typealias MIDIEntityRef

An entity that a device owns and that contains endpoints.


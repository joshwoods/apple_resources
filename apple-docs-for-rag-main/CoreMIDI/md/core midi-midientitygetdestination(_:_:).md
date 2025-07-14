

- Core MIDI
-  MIDIEntityGetDestination(\_:\_:) 

Function

# MIDIEntityGetDestination(\_:\_:)

Returns one of an entity’s destinations.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIEntityGetDestination(
    _ entity: MIDIEntityRef,
    _ destIndex0: Int
) -> MIDIEndpointRef
```

## Parameters 

`entity`  

The entity to query.

`destIndex0`  

The destination index.

## Return Value

A reference to a destination, or `NULL` if an error occurred.

## See Also

### Entity lookup

func MIDIEntityGetDevice(MIDIEntityRef, UnsafeMutablePointer&lt;MIDIDeviceRef>?) -> OSStatus

Returns an entity’s device.

func MIDIEntityGetNumberOfSources(MIDIEntityRef) -> Int

Returns the number of sources in an entity.

func MIDIEntityGetSource(MIDIEntityRef, Int) -> MIDIEndpointRef

Returns one of an entity’s sources.

func MIDIEntityGetNumberOfDestinations(MIDIEntityRef) -> Int

Returns the number of destinations in an entity.

typealias MIDIEntityRef

An entity that a device owns and that contains endpoints.




- Core MIDI
-  MIDIEntityGetSource(\_:\_:) 

Function

# MIDIEntityGetSource(\_:\_:)

Returns one of an entity’s sources.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIEntityGetSource(
    _ entity: MIDIEntityRef,
    _ sourceIndex0: Int
) -> MIDIEndpointRef
```

## Parameters 

`entity`  

The entity to query.

`sourceIndex0`  

The source index.

## Return Value

A reference to a source, or `NULL` if an error occurred.

## See Also

### Entity lookup

func MIDIEntityGetDevice(MIDIEntityRef, UnsafeMutablePointer&lt;MIDIDeviceRef>?) -> OSStatus

Returns an entity’s device.

func MIDIEntityGetNumberOfSources(MIDIEntityRef) -> Int

Returns the number of sources in an entity.

func MIDIEntityGetNumberOfDestinations(MIDIEntityRef) -> Int

Returns the number of destinations in an entity.

func MIDIEntityGetDestination(MIDIEntityRef, Int) -> MIDIEndpointRef

Returns one of an entity’s destinations.

typealias MIDIEntityRef

An entity that a device owns and that contains endpoints.


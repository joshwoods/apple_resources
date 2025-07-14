

- Core MIDI
-  MIDIEntityRef 

Type Alias

# MIDIEntityRef

An entity that a device owns and that contains endpoints.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias MIDIEntityRef = MIDIObjectRef
```

## Discussion

An entity object derives from MIDIObjectRef, and its owning object is a MIDIDeviceRef.

Devices may have multiple logically distinct subcomponents; for example, a MIDI synthesizer and a pair of MIDI ports are addressable using a USB port. By grouping a device’s endpoints into entities, the system has enough information for an app to make reasonable assumptions about how to communicate bidirectionally with each entity, as required by MIDI librarian apps.

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

func MIDIEntityGetDestination(MIDIEntityRef, Int) -> MIDIEndpointRef

Returns one of an entity’s destinations.


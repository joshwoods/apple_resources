

- Core MIDI
-  kMIDIPropertySingleRealtimeEntity 

Global Variable

# kMIDIPropertySingleRealtimeEntity

The 0-based index of the entity on which incoming real-time messages from the device appear to have originated.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.2+visionOS 1.0+

``` source
let kMIDIPropertySingleRealtimeEntity: CFString
```

## See Also

### Connections

let kMIDIPropertyCanRoute: CFString

A Boolean value that indicates whether the device or entity can route messages to or from external MIDI devices.

let kMIDIPropertyIsBroadcast: CFString

A Boolean value that indicates whether the endpoint broadcasts messages to all of the other endpoints in the device.

let kMIDIPropertyConnectionUniqueID: CFString

The unique identifier of an external device attached to this connection.

let kMIDIPropertyIsEmbeddedEntity: CFString

A Boolean value that indicates whether this entity or endpoint has external MIDI connections.


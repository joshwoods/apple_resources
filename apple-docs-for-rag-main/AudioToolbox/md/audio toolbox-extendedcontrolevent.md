

- Audio Toolbox
-  ExtendedControlEvent 

Structure

# ExtendedControlEvent

macOS

``` source
struct ExtendedControlEvent
```

## Topics

### Initializers

init()

init(groupID: MusicDeviceGroupID, controlID: AudioUnitParameterID, value: AudioUnitParameterValue)

### Instance Properties

var controlID: AudioUnitParameterID

var groupID: MusicDeviceGroupID

var value: AudioUnitParameterValue

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

typealias MIDIEndpointRef = MIDIObjectRef

A MIDI source or destination an entity owns.

typealias MagicCookieInfo

A structure holding magic cookie information.

Deprecated

typealias NoteInstanceID

typealias ReadBytesFDF

typealias ReadPacketDataFDF

typealias ReadPacketsFDF

typealias SetPropertyFDF

typealias SetUserDataFDF

typealias WriteBytesFDF

typealias WritePacketsFDF

typealias AudioSessionPropertyID

The data type for an audio session property identifier.

Deprecated


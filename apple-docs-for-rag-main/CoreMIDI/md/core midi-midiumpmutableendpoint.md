

- Core MIDI
-  MIDIUMPMutableEndpoint 

Class

# MIDIUMPMutableEndpoint

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
class MIDIUMPMutableEndpoint
```

## Topics

### Initializers

init?(name: String, deviceInfo: MIDI2DeviceInfo, productInstanceID: String, midiProtocol: MIDIProtocolID, destinationCallback: MIDIReceiveBlock)

### Instance Properties

var isEnabled: Bool

var mutableFunctionBlocks: [MIDIUMPMutableFunctionBlock]

### Instance Methods

func registerFunctionBlocks([MIDIUMPMutableFunctionBlock], markAsStatic: Bool) throws

func setEnabled(Bool) throws

func setName(String) throws

## Relationships

### Inherits From

- MIDIUMPEndpoint

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol


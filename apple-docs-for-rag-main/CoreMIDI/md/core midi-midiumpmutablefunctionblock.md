

- Core MIDI
-  MIDIUMPMutableFunctionBlock 

Class

# MIDIUMPMutableFunctionBlock

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
class MIDIUMPMutableFunctionBlock
```

## Topics

### Initializers

init?(name: String, direction: MIDIUMPFunctionBlockDirection, firstGroup: MIDIUMPGroupNumber, totalGroupsSpanned: MIDIUInteger7, maxSysEx8Streams: MIDIUInteger7, midi1Info: MIDIUMPFunctionBlockMIDI1Info, uiHint: MIDIUMPFunctionBlockUIHint, isEnabled: Bool)

### Instance Properties

var umpEndpoint: MIDIUMPMutableEndpoint?

### Instance Methods

func reconfigure(firstGroup: MIDIUMPGroupNumber, direction: MIDIUMPFunctionBlockDirection, MIDI1Info: MIDIUMPFunctionBlockMIDI1Info, UIHint: MIDIUMPFunctionBlockUIHint) throws

func setEnabled(Bool) throws

func setName(String) throws

## Relationships

### Inherits From

- MIDIUMPFunctionBlock

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol


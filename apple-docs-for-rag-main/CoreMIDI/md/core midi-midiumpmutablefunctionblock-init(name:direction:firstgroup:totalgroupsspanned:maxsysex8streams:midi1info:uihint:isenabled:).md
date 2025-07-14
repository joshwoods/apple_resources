

- Core MIDI
- MIDIUMPMutableFunctionBlock
-  init(name:direction:firstGroup:totalGroupsSpanned:maxSysEx8Streams:midi1Info:uiHint:isEnabled:) 

Initializer

# init(name:direction:firstGroup:totalGroupsSpanned:maxSysEx8Streams:midi1Info:uiHint:isEnabled:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init?(
    name: String,
    direction: MIDIUMPFunctionBlockDirection,
    firstGroup: MIDIUMPGroupNumber,
    totalGroupsSpanned: MIDIUInteger7,
    maxSysEx8Streams: MIDIUInteger7,
    midi1Info MIDI1Info: MIDIUMPFunctionBlockMIDI1Info,
    uiHint UIHint: MIDIUMPFunctionBlockUIHint,
    isEnabled: Bool
)
```


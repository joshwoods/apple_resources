

- Core MIDI
- MIDIUMPMutableEndpoint
-  init(name:deviceInfo:productInstanceID:midiProtocol:destinationCallback:) 

Initializer

# init(name:deviceInfo:productInstanceID:midiProtocol:destinationCallback:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init?(
    name: String,
    deviceInfo: MIDI2DeviceInfo,
    productInstanceID: String,
    midiProtocol MIDIProtocol: MIDIProtocolID,
    destinationCallback: @escaping MIDIReceiveBlock
)
```


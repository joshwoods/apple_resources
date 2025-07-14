

- Core MIDI
-  MIDIUMPEndpoint 

Class

# MIDIUMPEndpoint

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
class MIDIUMPEndpoint
```

## Topics

### Instance Properties

var deviceInfo: MIDI2DeviceInfo

var endpointType: MIDIUMPCIObjectBackingType

var functionBlocks: [MIDIUMPFunctionBlock]

var hasJRTSReceiveCapability: Bool

var hasJRTSTransmitCapability: Bool

var hasStaticFunctionBlocks: Bool

var midiDestination: MIDIEndpointRef

var midiProtocol: MIDIProtocolID

var midiSource: MIDIEndpointRef

var name: String

var productInstanceID: String

var supportedMIDIProtocols: MIDIUMPProtocolOptions

## Relationships

### Inherits From

- NSObject

### Inherited By

- MIDIUMPMutableEndpoint

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol


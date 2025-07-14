

- Core MIDI
- MIDINetworkSession
-  localName 

Instance Property

# localName

The name of this session’s entity.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var localName: String { get }
```

## Discussion

The session’s endpoints inherit this value.

## See Also

### Inspecting a Sessions

var networkName: String

The name with which this session advertises itself over Bonjour.

var networkPort: Int

The session’s UDP port.

func sourceEndpoint() -> MIDIEndpointRef

Returns the session’s source endpoint.

func destinationEndpoint() -> MIDIEndpointRef

Returns the session’s destination endpoint.


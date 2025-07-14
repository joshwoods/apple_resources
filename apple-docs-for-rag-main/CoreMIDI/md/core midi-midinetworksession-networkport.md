

- Core MIDI
- MIDINetworkSession
-  networkPort 

Instance Property

# networkPort

The session’s UDP port.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var networkPort: Int { get }
```

## See Also

### Inspecting a Sessions

var localName: String

The name of this session’s entity.

var networkName: String

The name with which this session advertises itself over Bonjour.

func sourceEndpoint() -> MIDIEndpointRef

Returns the session’s source endpoint.

func destinationEndpoint() -> MIDIEndpointRef

Returns the session’s destination endpoint.


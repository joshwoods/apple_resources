

- Core MIDI
- MIDINetworkSession
-  networkName 

Instance Property

# networkName

The name with which this session advertises itself over Bonjour.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var networkName: String { get }
```

## See Also

### Inspecting a Sessions

var localName: String

The name of this session’s entity.

var networkPort: Int

The session’s UDP port.

func sourceEndpoint() -> MIDIEndpointRef

Returns the session’s source endpoint.

func destinationEndpoint() -> MIDIEndpointRef

Returns the session’s destination endpoint.


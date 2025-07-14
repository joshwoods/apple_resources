

- Core MIDI
- MIDINetworkSession
-  destinationEndpoint() 

Instance Method

# destinationEndpoint()

Returns the session’s destination endpoint.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func destinationEndpoint() -> MIDIEndpointRef
```

## Return Value

The destination endpoint.

## See Also

### Inspecting a Sessions

var localName: String

The name of this session’s entity.

var networkName: String

The name with which this session advertises itself over Bonjour.

var networkPort: Int

The session’s UDP port.

func sourceEndpoint() -> MIDIEndpointRef

Returns the session’s source endpoint.




- Core MIDI
- MIDINetworkSession
-  connections() 

Instance Method

# connections()

Returns the session’s set of MIDI network connections.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func connections() -> Set
```

## Return Value

The set of connections.

## See Also

### Managing Connections

func addConnection(MIDINetworkConnection) -> Bool

Adds a new connection to this session.

func removeConnection(MIDINetworkConnection) -> Bool

Removes a connection from this session.


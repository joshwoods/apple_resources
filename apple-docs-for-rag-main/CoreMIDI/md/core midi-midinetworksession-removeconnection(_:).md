

- Core MIDI
- MIDINetworkSession
-  removeConnection(\_:) 

Instance Method

# removeConnection(\_:)

Removes a connection from this session.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func removeConnection(_ connection: MIDINetworkConnection) -> Bool
```

## Parameters 

`connection`  

The connection to remove.

## Return Value

true if the session successfully removed the connection, otherwise false.

## See Also

### Managing Connections

func connections() -> Set&lt;MIDINetworkConnection>

Returns the session’s set of MIDI network connections.

func addConnection(MIDINetworkConnection) -> Bool

Adds a new connection to this session.


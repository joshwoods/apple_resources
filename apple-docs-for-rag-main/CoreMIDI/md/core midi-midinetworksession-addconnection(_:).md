

- Core MIDI
- MIDINetworkSession
-  addConnection(\_:) 

Instance Method

# addConnection(\_:)

Adds a new connection to this session.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func addConnection(_ connection: MIDINetworkConnection) -> Bool
```

## Parameters 

`connection`  

The connection to add.

## Return Value

true if the session successfully added the connection, otherwise false.

## See Also

### Managing Connections

func connections() -> Set&lt;MIDINetworkConnection>

Returns the session’s set of MIDI network connections.

func removeConnection(MIDINetworkConnection) -> Bool

Removes a connection from this session.




- Core Media I/O
- CMIOExtensionProviderSource
-  disconnect(from:) 

Instance Method

# disconnect(from:)

Disconnects a client from a source’s provider.

Mac Catalyst 15.4+macOS 12.3+

``` source
func disconnect(from client: CMIOExtensionClient)
```

**Required**

## Parameters 

`client`  

A client to disconnect to the source’s provider.

## See Also

### Managing Connections

func connect(to: CMIOExtensionClient) throws

Connects a client to a source’s provider.

**Required**


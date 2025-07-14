

- Core Media I/O
- CMIOExtensionProviderSource
-  connect(to:) 

Instance Method

# connect(to:)

Connects a client to a source’s provider.

Mac Catalyst 15.4+macOS 12.3+

``` source
func connect(to client: CMIOExtensionClient) throws
```

**Required**

## Parameters 

`client`  

A client to connect to a source’s provider.

## See Also

### Managing Connections

func disconnect(from: CMIOExtensionClient)

Disconnects a client from a source’s provider.

**Required**


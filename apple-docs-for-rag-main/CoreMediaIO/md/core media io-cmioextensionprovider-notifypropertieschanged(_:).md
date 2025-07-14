

- Core Media I/O
- CMIOExtensionProvider
-  notifyPropertiesChanged(\_:) 

Instance Method

# notifyPropertiesChanged(\_:)

Notifies connected clients of device property changes.

Mac Catalyst 15.4+macOS 12.3+

``` source
func notifyPropertiesChanged(_ propertyStates: [CMIOExtensionProperty : CMIOExtensionPropertyState])
```

## Parameters 

`propertyStates`  

A dictionary of properties with changes.

## See Also

### Managing Clients

var connectedClients: [CMIOExtensionClient]

An array of connected clients.


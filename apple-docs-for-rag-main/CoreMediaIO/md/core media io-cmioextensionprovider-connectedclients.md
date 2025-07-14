

- Core Media I/O
- CMIOExtensionProvider
-  connectedClients 

Instance Property

# connectedClients

An array of connected clients.

Mac Catalyst 15.4+macOS 12.3+

``` source
var connectedClients: [CMIOExtensionClient] { get }
```

## Discussion

This property is key-value observable.

## See Also

### Managing Clients

func notifyPropertiesChanged([CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>])

Notifies connected clients of device property changes.




- ExtensionKit
- EXHostViewController
-  makeXPCConnection() 

Instance Method

# makeXPCConnection()

Attempts to connect to the extension over XPC.

macOS 13.0+

``` source
@MainActor
func makeXPCConnection() throws -> NSXPCConnection
```

## Return Value

An object representing the connection.

## See Also

### Connecting to the Extension

var delegate: (any EXHostViewControllerDelegate)?

The connection delegate.

protocol EXHostViewControllerDelegate

The delegate for a hosted view controller.




- ExtensionKit
- EXHostViewController
-  delegate 

Instance Property

# delegate

The connection delegate.

macOS 13.0+

``` source
@MainActor
weak var delegate: (any EXHostViewControllerDelegate)? { get set }
```

## See Also

### Connecting to the Extension

func makeXPCConnection() throws -> NSXPCConnection

Attempts to connect to the extension over XPC.

protocol EXHostViewControllerDelegate

The delegate for a hosted view controller.


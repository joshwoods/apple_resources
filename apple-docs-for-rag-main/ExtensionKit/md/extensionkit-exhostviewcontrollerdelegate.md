

- ExtensionKit
-  EXHostViewControllerDelegate 

Protocol

# EXHostViewControllerDelegate

The delegate for a hosted view controller.

macOS 13.0+

``` source
protocol EXHostViewControllerDelegate : NSObjectProtocol
```

## Topics

### Delegate Methods

func hostViewControllerDidActivate(EXHostViewController)

A delegate method the view controller calls when a connection succeeds.

func hostViewControllerWillDeactivate(EXHostViewController, error: (any Error)?)

A delegate method the host view controller calls when an extension disconnects.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Connecting to the Extension

func makeXPCConnection() throws -> NSXPCConnection

Attempts to connect to the extension over XPC.

var delegate: (any EXHostViewControllerDelegate)?

The connection delegate.


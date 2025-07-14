

- ExtensionKit
-  EXHostViewController 

Class

# EXHostViewController

A view controller that hosts remote views provided by an extension.

macOS 13.0+

``` source
@MainActor
class EXHostViewController
```

## Topics

### Configuring the View Controller

var configuration: EXHostViewController.Configuration?

The view controller’s configuration.

struct Configuration

An object that holds configuration options for a host view controller.

var placeholderView: NSView

A view that’s used when the view controller has no content to display.

### Connecting to the Extension

func makeXPCConnection() throws -> NSXPCConnection

Attempts to connect to the extension over XPC.

var delegate: (any EXHostViewControllerDelegate)?

The connection delegate.

protocol EXHostViewControllerDelegate

The delegate for a hosted view controller.

## Relationships

### Inherits From

- NSViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Host Apps

class EXAppExtensionBrowserViewController

A view controller that allows users to enable and disable extensions.


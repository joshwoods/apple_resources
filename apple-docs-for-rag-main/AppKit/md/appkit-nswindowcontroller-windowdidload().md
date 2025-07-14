

- AppKit
- NSWindowController
-  windowDidLoad() 

Instance Method

# windowDidLoad()

Sent after the window owned by the receiver has been loaded.

macOS

``` source
@MainActor
func windowDidLoad()
```

## Discussion

The default implementation does nothing.

## See Also

### Related Documentation

class NSWindowController

A controller that manages a window, usually a window stored in a nib file.

### Loading and Displaying the Window

func loadWindow()

Loads the receiver’s window from the nib file.

func showWindow(Any?)

Displays the window associated with the receiver.

var isWindowLoaded: Bool

A Boolean value that indicates whether the nib file containing the receiver’s window has been loaded.

var window: NSWindow?

The window owned by the receiver.

func windowWillLoad()

Sent before the window owned by the receiver is loaded.


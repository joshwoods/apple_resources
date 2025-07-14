

- AppKit
- NSWindowController
-  loadWindow() 

Instance Method

# loadWindow()

Loads the receiver’s window from the nib file.

macOS

``` source
@MainActor
func loadWindow()
```

## Discussion

You should never directly invoke this method. Instead, access the window property so the windowDidLoad() and windowWillLoad() methods are invoked. Subclasses can override this method if the way it finds and loads the window is not adequate. It uses the Bundle class’s init(for:) method to get the bundle, using the class of the nib file owner as argument. It then locates the nib file within the bundle and, if successful, loads it; if unsuccessful, it tries to find the nib file in the main bundle.

## See Also

### Loading and Displaying the Window

func showWindow(Any?)

Displays the window associated with the receiver.

var isWindowLoaded: Bool

A Boolean value that indicates whether the nib file containing the receiver’s window has been loaded.

var window: NSWindow?

The window owned by the receiver.

func windowDidLoad()

Sent after the window owned by the receiver has been loaded.

func windowWillLoad()

Sent before the window owned by the receiver is loaded.


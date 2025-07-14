

- AppKit
- NSWindowController
-  isWindowLoaded 

Instance Property

# isWindowLoaded

A Boolean value that indicates whether the nib file containing the receiver’s window has been loaded.

macOS

``` source
@MainActor
var isWindowLoaded: Bool { get }
```

## Discussion

The value of this property is true if the nib file containing the receiver’s window has been loaded, false otherwise.

## See Also

### Loading and Displaying the Window

func loadWindow()

Loads the receiver’s window from the nib file.

func showWindow(Any?)

Displays the window associated with the receiver.

var window: NSWindow?

The window owned by the receiver.

func windowDidLoad()

Sent after the window owned by the receiver has been loaded.

func windowWillLoad()

Sent before the window owned by the receiver is loaded.


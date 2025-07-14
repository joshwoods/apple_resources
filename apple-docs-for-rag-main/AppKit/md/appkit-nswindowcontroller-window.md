

- AppKit
- NSWindowController
-  window 

Instance Property

# window

The window owned by the receiver.

macOS

``` source
@MainActor
var window: NSWindow? { get set }
```

## Discussion

Accessing this property loads the nib file if there is one and it has not yet been loaded. If the window was loaded, the following methods are called in order: windowWillLoad(), loadWindow(), and windowDidLoad(). If the window controller has a document, the document’s corresponding methods windowControllerWillLoadNib(_:) and windowControllerDidLoadNib(_:) are also called (if implemented). To affect nib loading or do something before or after it happens, you should always override these methods.

Setting this property releases the window controller’s old window along with any associated top-level objects in its nib file, and establishes ownership of the specified new window. Typically, you should not use this property to set the window. Instead, create a new window controller for the new window and then release the old window controller.

## See Also

### Related Documentation

func windowControllerWillLoadNib(NSWindowController)

Called before one of the document’s window controllers loads its nib file.

### Loading and Displaying the Window

func loadWindow()

Loads the receiver’s window from the nib file.

func showWindow(Any?)

Displays the window associated with the receiver.

var isWindowLoaded: Bool

A Boolean value that indicates whether the nib file containing the receiver’s window has been loaded.

func windowDidLoad()

Sent after the window owned by the receiver has been loaded.

func windowWillLoad()

Sent before the window owned by the receiver is loaded.


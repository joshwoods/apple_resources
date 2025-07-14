

- AppKit
- NSDocument
-  windowNibName 

Instance Property

# windowNibName

The name of the document’s sole nib file.

macOS

``` source
@MainActor
var windowNibName: NSNib.Name? { get }
```

## Discussion

Using this name, `NSDocument` creates and instantiates a default instance of `NSWindowController` to manage the window. If your document has multiple nib files, each with its own single window, or if the default `NSWindowController` instance is not adequate for your purposes, you should override makeWindowControllers().

The default value of this property is `nil`. Subclasses must override it to specify a nib file name.

## See Also

### Creating and Managing Window Controllers

func makeWindowControllers()

Creates the window controller objects that the document uses to display its content.

func addWindowController(NSWindowController)

Adds the specified window controller to the current document.

func removeWindowController(NSWindowController)

Removes the specified window controller from the receiver’s array of window controllers.

var windowControllers: [NSWindowController]

The document’s current window controllers.

func windowControllerDidLoadNib(NSWindowController)

Called after one of the document’s window controllers loads its nib file.

func windowControllerWillLoadNib(NSWindowController)

Called before one of the document’s window controllers loads its nib file.

func shouldCloseWindowController(NSWindowController, delegate: Any?, shouldClose: Selector?, contextInfo: UnsafeMutableRawPointer?)

Determines whether the system should close the document and its associated window.


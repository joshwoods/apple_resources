

- AppKit
- NSDocument
-  windowControllers 

Instance Property

# windowControllers

The document’s current window controllers.

macOS

``` source
@MainActor
var windowControllers: [NSWindowController] { get }
```

## Discussion

The value of this property is an array of NSWindowController objects belonging to the current document. If there are no window controllers, the value is an empty array object.

## See Also

### Creating and Managing Window Controllers

func makeWindowControllers()

Creates the window controller objects that the document uses to display its content.

func addWindowController(NSWindowController)

Adds the specified window controller to the current document.

func removeWindowController(NSWindowController)

Removes the specified window controller from the receiver’s array of window controllers.

var windowNibName: NSNib.Name?

The name of the document’s sole nib file.

func windowControllerDidLoadNib(NSWindowController)

Called after one of the document’s window controllers loads its nib file.

func windowControllerWillLoadNib(NSWindowController)

Called before one of the document’s window controllers loads its nib file.

func shouldCloseWindowController(NSWindowController, delegate: Any?, shouldClose: Selector?, contextInfo: UnsafeMutableRawPointer?)

Determines whether the system should close the document and its associated window.




- AppKit
- NSDocument
-  makeWindowControllers() 

Instance Method

# makeWindowControllers()

Creates the window controller objects that the document uses to display its content.

macOS

``` source
@MainActor
func makeWindowControllers()
```

## Discussion

Subclasses may override this method to create the initial window controller(s) for the document.

The base class implementation creates an `NSWindowController` object with windowNibName and with the document as the file’s owner if windowNibName returns a name. If you override this method to create your own window controllers, be sure to use addWindowController(_:) to add them to the document after creating them.

This method is called by the `NSDocumentController` `open...` methods, but you might want to call it directly in some circumstances.

## See Also

### Creating and Managing Window Controllers

func addWindowController(NSWindowController)

Adds the specified window controller to the current document.

func removeWindowController(NSWindowController)

Removes the specified window controller from the receiver’s array of window controllers.

var windowControllers: [NSWindowController]

The document’s current window controllers.

var windowNibName: NSNib.Name?

The name of the document’s sole nib file.

func windowControllerDidLoadNib(NSWindowController)

Called after one of the document’s window controllers loads its nib file.

func windowControllerWillLoadNib(NSWindowController)

Called before one of the document’s window controllers loads its nib file.

func shouldCloseWindowController(NSWindowController, delegate: Any?, shouldClose: Selector?, contextInfo: UnsafeMutableRawPointer?)

Determines whether the system should close the document and its associated window.


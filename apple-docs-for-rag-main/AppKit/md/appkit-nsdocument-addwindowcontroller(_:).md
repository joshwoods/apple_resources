

- AppKit
- NSDocument
-  addWindowController(\_:) 

Instance Method

# addWindowController(\_:)

Adds the specified window controller to the current document.

macOS

``` source
@MainActor
func addWindowController(_ windowController: NSWindowController)
```

## Parameters 

`windowController`  

The window controller that is added.

## Discussion

An NSDocument object uses its list of window controllers when it displays all document windows, sets window edited status upon an undo or redo operation, and modifies window titles. If you create window controllers by overriding windowNibName, this method is invoked automatically. If you create window controllers in makeWindowControllers() or in any other context, such as in apps that present multiple windows per document, you should invoke this method for each window controller created.

You cannot attach a window controller to more than one document at a time. The default implementation of this method removes the passed-in window controller from the document to which it is attached, if it is already attached to one, then sends it a document message with `self` as the argument. It also ignores redundant invocations.

You would not typically override this method.

## See Also

### Related Documentation

var document: AnyObject?

The document associated with the window controller.

### Creating and Managing Window Controllers

func makeWindowControllers()

Creates the window controller objects that the document uses to display its content.

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


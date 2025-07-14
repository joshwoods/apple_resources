

- AppKit
- NSDocument
-  removeWindowController(\_:) 

Instance Method

# removeWindowController(\_:)

Removes the specified window controller from the receiver’s array of window controllers.

macOS

``` source
@MainActor
func removeWindowController(_ windowController: NSWindowController)
```

## Parameters 

`windowController`  

The window controller that is removed.

## Discussion

A document with no window controllers is not necessarily closed. However, a window controller can be set to close its associated document when the window is closed or the window controller is deallocated.

The default implementation of this method sends a document message to the passed-in window controller with a `nil` argument. You would not typically override this method.

## See Also

### Related Documentation

var shouldCloseDocument: Bool

A Boolean value that indicates whether the receiver necessarily closes the associated document when the window it manages is closed.

### Creating and Managing Window Controllers

func makeWindowControllers()

Creates the window controller objects that the document uses to display its content.

func addWindowController(NSWindowController)

Adds the specified window controller to the current document.

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


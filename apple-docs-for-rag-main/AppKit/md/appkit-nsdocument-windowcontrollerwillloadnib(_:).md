

- AppKit
- NSDocument
-  windowControllerWillLoadNib(\_:) 

Instance Method

# windowControllerWillLoadNib(\_:)

Called before one of the document’s window controllers loads its nib file.

macOS

``` source
@MainActor
func windowControllerWillLoadNib(_ windowController: NSWindowController)
```

## Parameters 

`windowController`  

The window controller that loads the nib file.

## Discussion

See the class description for NSWindowController for additional information about nib files and the file’s owner object.

Typically an `NSDocument` subclass overrides windowNibName or makeWindowControllers(), but not both. If windowNibName is overridden, the default implementation of makeWindowControllers() will load the named nib file, making the NSDocument the nib file’s owner. In that case, you can override windowControllerWillLoadNib(_:) and do custom processing before the nib file is loaded.

The default implementation of this method does nothing.

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

var windowNibName: NSNib.Name?

The name of the document’s sole nib file.

func windowControllerDidLoadNib(NSWindowController)

Called after one of the document’s window controllers loads its nib file.

func shouldCloseWindowController(NSWindowController, delegate: Any?, shouldClose: Selector?, contextInfo: UnsafeMutableRawPointer?)

Determines whether the system should close the document and its associated window.


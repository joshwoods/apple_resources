

- AppKit
- NSWindowController
-  synchronizeWindowTitleWithDocumentName() 

Instance Method

# synchronizeWindowTitleWithDocumentName()

Synchronizes the displayed window title and the represented filename with the information in the associated document.

macOS

``` source
@MainActor
func synchronizeWindowTitleWithDocumentName()
```

## Discussion

Does nothing if the window controller has no associated document or loaded window. This method queries the window controller’s document to get the document’s display name and full filename path, then calls windowTitle(forDocumentDisplayName:) to get the display name to show in the window title.

## See Also

### Accessing Window Attributes and Content

var shouldCascadeWindows: Bool

A Boolean value that indicates whether the window will cascade in relation to other document windows when it is displayed.

var windowFrameAutosaveName: NSWindow.FrameAutosaveName

The name under which the frame rectangle of the window owned by the receiver is stored in the defaults database.

func windowTitle(forDocumentDisplayName: String) -> String

Returns the window title to be used for a given document display name.

var contentViewController: NSViewController?

The view controller for the window’s content view.

func dismissController(Any?)

Dismisses the window controller.


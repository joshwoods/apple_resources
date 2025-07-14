

- AppKit
- NSWindowController
-  shouldCascadeWindows 

Instance Property

# shouldCascadeWindows

A Boolean value that indicates whether the window will cascade in relation to other document windows when it is displayed.

macOS

``` source
@MainActor
var shouldCascadeWindows: Bool { get set }
```

## Discussion

Cascading in relation to other document windows means having a slightly offset location so that the title bars of previously displayed windows are still visible. The value of this property is true if the window will cascade in relation to other document windows, false otherwise. The default value is true.

## See Also

### Accessing Window Attributes and Content

var windowFrameAutosaveName: NSWindow.FrameAutosaveName

The name under which the frame rectangle of the window owned by the receiver is stored in the defaults database.

func synchronizeWindowTitleWithDocumentName()

Synchronizes the displayed window title and the represented filename with the information in the associated document.

func windowTitle(forDocumentDisplayName: String) -> String

Returns the window title to be used for a given document display name.

var contentViewController: NSViewController?

The view controller for the window’s content view.

func dismissController(Any?)

Dismisses the window controller.


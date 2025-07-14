

- AppKit
- NSWindowController
-  contentViewController 

Instance Property

# contentViewController

The view controller for the window’s content view.

macOS 10.10+

``` source
@MainActor
var contentViewController: NSViewController? { get set }
```

## Discussion

The value of this property tracks the window’s contentView property.

## See Also

### Accessing Window Attributes and Content

var shouldCascadeWindows: Bool

A Boolean value that indicates whether the window will cascade in relation to other document windows when it is displayed.

var windowFrameAutosaveName: NSWindow.FrameAutosaveName

The name under which the frame rectangle of the window owned by the receiver is stored in the defaults database.

func synchronizeWindowTitleWithDocumentName()

Synchronizes the displayed window title and the represented filename with the information in the associated document.

func windowTitle(forDocumentDisplayName: String) -> String

Returns the window title to be used for a given document display name.

func dismissController(Any?)

Dismisses the window controller.




- AppKit
- NSWindowController
-  windowFrameAutosaveName 

Instance Property

# windowFrameAutosaveName

The name under which the frame rectangle of the window owned by the receiver is stored in the defaults database.

macOS

``` source
@MainActor
var windowFrameAutosaveName: NSWindow.FrameAutosaveName { get set }
```

## Discussion

By default, `name` is an empty string, which means that no information is stored in the defaults database.

## See Also

### Related Documentation

func setFrameAutosaveName(NSWindow.FrameAutosaveName) -> Bool

Sets the name AppKit uses to automatically save the window’s frame rectangle data in the defaults system.

### Accessing Window Attributes and Content

var shouldCascadeWindows: Bool

A Boolean value that indicates whether the window will cascade in relation to other document windows when it is displayed.

func synchronizeWindowTitleWithDocumentName()

Synchronizes the displayed window title and the represented filename with the information in the associated document.

func windowTitle(forDocumentDisplayName: String) -> String

Returns the window title to be used for a given document display name.

var contentViewController: NSViewController?

The view controller for the window’s content view.

func dismissController(Any?)

Dismisses the window controller.


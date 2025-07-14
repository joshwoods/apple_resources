

- AppKit
- NSWindowController
-  windowTitle(forDocumentDisplayName:) 

Instance Method

# windowTitle(forDocumentDisplayName:)

Returns the window title to be used for a given document display name.

macOS

``` source
@MainActor
func windowTitle(forDocumentDisplayName displayName: String) -> String
```

## Parameters 

`displayName`  

The display name for the document. This is the last path component under which the document file is saved.

## Discussion

The default implementation returns `displayName`. Subclasses can override this method to customize the window title. For example, a CAD application could append “-Top” or “-Side,” depending on the view displayed by the window.

## See Also

### Accessing Window Attributes and Content

var shouldCascadeWindows: Bool

A Boolean value that indicates whether the window will cascade in relation to other document windows when it is displayed.

var windowFrameAutosaveName: NSWindow.FrameAutosaveName

The name under which the frame rectangle of the window owned by the receiver is stored in the defaults database.

func synchronizeWindowTitleWithDocumentName()

Synchronizes the displayed window title and the represented filename with the information in the associated document.

var contentViewController: NSViewController?

The view controller for the window’s content view.

func dismissController(Any?)

Dismisses the window controller.


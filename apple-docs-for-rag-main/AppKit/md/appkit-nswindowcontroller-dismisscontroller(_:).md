

- AppKit
- NSWindowController
-  dismissController(\_:) 

Instance Method

# dismissController(\_:)

Dismisses the window controller.

macOS 10.10+

``` source
@IBAction @MainActor
func dismissController(_ sender: Any?)
```

## Parameters 

`sender`  

The sender of the message.

## Discussion

This method does nothing if the receiver is not currently presented.

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

var contentViewController: NSViewController?

The view controller for the window’s content view.




- AppKit
- NSResponder
-  newWindowForTab(\_:) 

Instance Method

# newWindowForTab(\_:)

Creates a new window to show as a tab in a tabbed window.

macOS 10.12+

``` source
@IBAction @MainActor
func newWindowForTab(_ sender: Any?)
```

## Parameters 

`sender`  

The sender of the action.

## Discussion

The system automatically calls this method to create a window for a new tab when the user clicks the plus button in a tabbed window. The system shows a plus button on a tabbed window only if this method exists on one of the following objects:

- In an NSDocumentController subclass

- In the responder chain starting at NSWindow, such as NSWindow, the window delegate, the window controller, the NSApplication delegate, and so on


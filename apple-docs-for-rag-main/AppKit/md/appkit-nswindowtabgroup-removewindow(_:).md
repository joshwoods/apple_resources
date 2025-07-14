

- AppKit
- NSWindowTabGroup
-  removeWindow(\_:) 

Instance Method

# removeWindow(\_:)

Removes a window from the tab group.

macOS 10.13+

``` source
func removeWindow(_ window: NSWindow)
```

## Parameters 

`window`  

The window to remove from the tab group. This window must already be a member of the tab group.

Raises an `NSInternalInconsistencyException` if the window is not a member of the tab group.

## Discussion

You can use removeWindow(_:) to explicitly remove a window from the tab group. Windows are implicity removed from their associated tab groups when they order out.

## See Also

### Managing Tabbed Windows

var windows: [NSWindow]

A collection of the windows that are currently grouped together by this window tab group.

var selectedWindow: NSWindow?

The selected, or frontmost, window in the tab group.

func addWindow(NSWindow)

Adds a window to the tab group.

func insertWindow(NSWindow, at: Int)

Inserts a window at a specific location within the tab group.


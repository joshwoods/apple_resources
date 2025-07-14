

- AppKit
- NSWindowTabGroup
-  selectedWindow 

Instance Property

# selectedWindow

The selected, or frontmost, window in the tab group.

macOS 10.13+

``` source
weak var selectedWindow: NSWindow? { get set }
```

## Discussion

This property returns the currently selected window within the tabbed window group. Setting this property visually changes the selected tab.

Important

This property raises an exception if set to a window that is not already a member of the tab group.

You can monitor this property for changes using key-value observing.

## See Also

### Managing Tabbed Windows

var windows: [NSWindow]

A collection of the windows that are currently grouped together by this window tab group.

func addWindow(NSWindow)

Adds a window to the tab group.

func insertWindow(NSWindow, at: Int)

Inserts a window at a specific location within the tab group.

func removeWindow(NSWindow)

Removes a window from the tab group.


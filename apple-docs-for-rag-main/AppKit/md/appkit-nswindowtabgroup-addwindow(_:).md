

- AppKit
- NSWindowTabGroup
-  addWindow(\_:) 

Instance Method

# addWindow(\_:)

Adds a window to the tab group.

macOS 10.13+

``` source
func addWindow(_ window: NSWindow)
```

## Parameters 

`window`  

The window to append to the tab group.

## Discussion

This method appends the window to the end of the tab group. If the window is already a member of another tab group, it is first removed from that group.

## See Also

### Managing Tabbed Windows

var windows: [NSWindow]

A collection of the windows that are currently grouped together by this window tab group.

var selectedWindow: NSWindow?

The selected, or frontmost, window in the tab group.

func insertWindow(NSWindow, at: Int)

Inserts a window at a specific location within the tab group.

func removeWindow(NSWindow)

Removes a window from the tab group.


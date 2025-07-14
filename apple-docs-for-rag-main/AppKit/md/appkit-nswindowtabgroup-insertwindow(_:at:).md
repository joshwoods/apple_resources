

- AppKit
- NSWindowTabGroup
-  insertWindow(\_:at:) 

Instance Method

# insertWindow(\_:at:)

Inserts a window at a specific location within the tab group.

macOS 10.13+

``` source
func insertWindow(
    _ window: NSWindow,
    at index: Int
)
```

## Parameters 

`window`  

The window to insert into the tab group.

`index`  

The location in the tab group at which to insert window. This value must not be negative, and must not be greater than the number of windows in the tab group.

Raises an `NSInternalInconsistencyException` if the index is negative or larger than the number of tabs in the group.

## Discussion

Inserts the window at the specified location within the tab group. If the window is already a member of another tab group, it is first removed from that group.

## See Also

### Managing Tabbed Windows

var windows: [NSWindow]

A collection of the windows that are currently grouped together by this window tab group.

var selectedWindow: NSWindow?

The selected, or frontmost, window in the tab group.

func addWindow(NSWindow)

Adds a window to the tab group.

func removeWindow(NSWindow)

Removes a window from the tab group.


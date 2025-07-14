

- AppKit
- NSWindowTabGroup
-  windows 

Instance Property

# windows

A collection of the windows that are currently grouped together by this window tab group.

macOS 10.13+

``` source
var windows: [NSWindow] { get }
```

## Discussion

The order of this array corresponds to the visual order of the tabs in this tab group, arranged from the leading edge of the tab bar to the trailing edge. You can monitor this property for changes using key-value observing.

## See Also

### Managing Tabbed Windows

var selectedWindow: NSWindow?

The selected, or frontmost, window in the tab group.

func addWindow(NSWindow)

Adds a window to the tab group.

func insertWindow(NSWindow, at: Int)

Inserts a window at a specific location within the tab group.

func removeWindow(NSWindow)

Removes a window from the tab group.


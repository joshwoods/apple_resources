

- AppKit
- NSApplication
-  removeWindowsItem(\_:) 

Instance Method

# removeWindowsItem(\_:)

Removes the Window menu item for a given window.

macOS

``` source
@MainActor
func removeWindowsItem(_ win: NSWindow)
```

## Parameters 

`win`  

The window whose menu item is to be removed.

## Discussion

This method doesn’t prevent the item from being automatically added again. Use the isExcludedFromWindowsMenu method of NSWindow if you want the item to remain excluded from the Window menu.

## See Also

### Managing the Window Menu

var windowsMenu: NSMenu?

The Window menu of the app.

func addWindowsItem(NSWindow, title: String, filename: Bool)

Adds an item to the Window menu for a given window.

func changeWindowsItem(NSWindow, title: String, filename: Bool)

Changes the item for a given window in the Window menu to a given string.

func updateWindowsItem(NSWindow)

Updates the Window menu item for a given window to reflect the edited status of that window.


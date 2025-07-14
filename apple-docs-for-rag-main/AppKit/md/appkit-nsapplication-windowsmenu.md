

- AppKit
- NSApplication
-  windowsMenu 

Instance Property

# windowsMenu

The Window menu of the app.

macOS

``` source
@MainActor
var windowsMenu: NSMenu? { get set }
```

## Return Value

The window menu or `nil` if such a menu does not exist or has not yet been created.

## Discussion

This property contains the app’s Window menu or `nil` if such a menu does not yet exist or has not yet been created. You can use this property to specify the Window menu for your app.

## See Also

### Managing the Window Menu

func addWindowsItem(NSWindow, title: String, filename: Bool)

Adds an item to the Window menu for a given window.

func changeWindowsItem(NSWindow, title: String, filename: Bool)

Changes the item for a given window in the Window menu to a given string.

func removeWindowsItem(NSWindow)

Removes the Window menu item for a given window.

func updateWindowsItem(NSWindow)

Updates the Window menu item for a given window to reflect the edited status of that window.




- AppKit
- NSApplication
-  updateWindowsItem(\_:) 

Instance Method

# updateWindowsItem(\_:)

Updates the Window menu item for a given window to reflect the edited status of that window.

macOS

``` source
@MainActor
func updateWindowsItem(_ win: NSWindow)
```

## Parameters 

`win`  

The window whose menu item is to be updated.

## Discussion

You rarely need to invoke this method because it is invoked automatically when the edit status of an NSWindow object is set.

## See Also

### Related Documentation

var isDocumentEdited: Bool

A Boolean value that indicates whether the window’s document has been edited.

### Managing the Window Menu

var windowsMenu: NSMenu?

The Window menu of the app.

func addWindowsItem(NSWindow, title: String, filename: Bool)

Adds an item to the Window menu for a given window.

func changeWindowsItem(NSWindow, title: String, filename: Bool)

Changes the item for a given window in the Window menu to a given string.

func removeWindowsItem(NSWindow)

Removes the Window menu item for a given window.


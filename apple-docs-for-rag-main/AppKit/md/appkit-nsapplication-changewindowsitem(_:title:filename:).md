

- AppKit
- NSApplication
-  changeWindowsItem(\_:title:filename:) 

Instance Method

# changeWindowsItem(\_:title:filename:)

Changes the item for a given window in the Window menu to a given string.

macOS

``` source
@MainActor
func changeWindowsItem(
    _ win: NSWindow,
    title string: String,
    filename isFilename: Bool
)
```

## Parameters 

`win`  

The window whose title you want to change in the Window menu. If `aWindow` is not in the Window menu, this method adds it.

`string`  

The string to display for the window’s menu item. How the string is interpreted is dependent on the value in the `isFilename` parameter.

`isFilename`  

If false, `aString` appears literally in the menu; otherwise, `aString` is assumed to be a converted pathname with the name of the file preceding the path (the way the `NSWindow` method setTitleWithRepresentedFilename(_:) shows a title)

## See Also

### Related Documentation

var title: String

The string that appears in the title bar of the window or the path to the represented file.

### Managing the Window Menu

var windowsMenu: NSMenu?

The Window menu of the app.

func addWindowsItem(NSWindow, title: String, filename: Bool)

Adds an item to the Window menu for a given window.

func removeWindowsItem(NSWindow)

Removes the Window menu item for a given window.

func updateWindowsItem(NSWindow)

Updates the Window menu item for a given window to reflect the edited status of that window.


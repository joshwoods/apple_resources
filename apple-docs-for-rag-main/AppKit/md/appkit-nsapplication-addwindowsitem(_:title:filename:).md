

- AppKit
- NSApplication
-  addWindowsItem(\_:title:filename:) 

Instance Method

# addWindowsItem(\_:title:filename:)

Adds an item to the Window menu for a given window.

macOS

``` source
@MainActor
func addWindowsItem(
    _ win: NSWindow,
    title string: String,
    filename isFilename: Bool
)
```

## Parameters 

`win`  

The window being added to the menu. If this window object already exists in the Window menu, this method has no effect.

`string`  

The string to display for the window’s menu item. How the string is interpreted is dependent on the value in the `isFilename` parameter.

`isFilename`  

If false, `aString` appears literally in the menu; otherwise, `aString` is assumed to be a converted pathname with the name of the file preceding the path (the way the `NSWindow` method setTitleWithRepresentedFilename(_:) shows a title)

## Discussion

You rarely need to invoke this method directly because Cocoa places an item in the Window menu automatically whenever you set the title of an `NSWindow` object.

## See Also

### Related Documentation

var title: String

The string that appears in the title bar of the window or the path to the represented file.

### Managing the Window Menu

var windowsMenu: NSMenu?

The Window menu of the app.

func changeWindowsItem(NSWindow, title: String, filename: Bool)

Changes the item for a given window in the Window menu to a given string.

func removeWindowsItem(NSWindow)

Removes the Window menu item for a given window.

func updateWindowsItem(NSWindow)

Updates the Window menu item for a given window to reflect the edited status of that window.


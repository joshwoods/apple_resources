

- AppKit
- NSWindow
-  standardWindowButton(\_:) 

Instance Method

# standardWindowButton(\_:)

Returns the window button of a given window button kind in the window’s view hierarchy.

macOS

``` source
@MainActor
func standardWindowButton(_ b: NSWindow.ButtonType) -> NSButton?
```

## Parameters 

`b`  

The type of standard window button to return.

## Return Value

Window button in the window’s view hierarchy of the type identified by `b`; `nil` when such button is not in the window’s view hierarchy.

## See Also

### Managing Title Bars

class func standardWindowButton(NSWindow.ButtonType, for: NSWindow.StyleMask) -> NSButton?

Returns a new instance of a given standard window button, sized appropriately for a given window style.

var showsToolbarButton: Bool

A Boolean value that indicates whether the toolbar control button is currently displayed.

Deprecated

var titlebarAppearsTransparent: Bool

A Boolean value that indicates whether the title bar draws its background.

var toolbarStyle: NSWindow.ToolbarStyle

The style that determines the appearance and location of the toolbar in relation to the title bar.

enum ToolbarStyle

Styles that determine the appearance and location of the toolbar in relation to the title bar.

var titlebarSeparatorStyle: NSTitlebarSeparatorStyle

The type of separator that the app displays between the title bar and content of a window.

enum NSTitlebarSeparatorStyle

Styles that determine the type of separator displayed between the title bar and content of a window.

var windowTitlebarLayoutDirection: NSUserInterfaceLayoutDirection

The direction the window’s title bar lays text out, either left to right or right to left.


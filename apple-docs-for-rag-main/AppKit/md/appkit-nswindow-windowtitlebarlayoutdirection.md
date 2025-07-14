

- AppKit
- NSWindow
-  windowTitlebarLayoutDirection 

Instance Property

# windowTitlebarLayoutDirection

The direction the window’s title bar lays text out, either left to right or right to left.

macOS 10.12+

``` source
@MainActor
var windowTitlebarLayoutDirection: NSUserInterfaceLayoutDirection { get }
```

## Discussion

The layout direction of the window title bar includes the standard window buttons (close, minimize, maximize) and the title for the window. In general, this returns NSUserInterfaceLayoutDirection.rightToLeft if the primary system language is right to left. The layout direction may be right to left even in applications that don’t have a right to left language localization. Refer to this value if the application uses titlebarAppearsTransparent and places controls under the title bar.

## See Also

### Managing Title Bars

class func standardWindowButton(NSWindow.ButtonType, for: NSWindow.StyleMask) -> NSButton?

Returns a new instance of a given standard window button, sized appropriately for a given window style.

func standardWindowButton(NSWindow.ButtonType) -> NSButton?

Returns the window button of a given window button kind in the window’s view hierarchy.

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


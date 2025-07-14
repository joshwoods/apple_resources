

- AppKit
- NSWindow
-  showsToolbarButton Deprecated

Instance Property

# showsToolbarButton

A Boolean value that indicates whether the toolbar control button is currently displayed.

macOS 10.0–15.4Deprecated

``` source
@MainActor
var showsToolbarButton: Bool { get set }
```

Deprecated

This property has no effect

## Discussion

The value of this property is true if the standard toolbar button is currently displayed; otherwise, false. When clicked, the toolbar control button shows or hides a window’s toolbar. The toolbar control button appears in a window’s title bar. If the window does not have a toolbar, this property has no effect.

## See Also

### Managing Title Bars

class func standardWindowButton(NSWindow.ButtonType, for: NSWindow.StyleMask) -> NSButton?

Returns a new instance of a given standard window button, sized appropriately for a given window style.

func standardWindowButton(NSWindow.ButtonType) -> NSButton?

Returns the window button of a given window button kind in the window’s view hierarchy.

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


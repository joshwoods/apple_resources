

- AppKit
- NSWindow
-  titlebarAppearsTransparent 

Instance Property

# titlebarAppearsTransparent

A Boolean value that indicates whether the title bar draws its background.

macOS 10.10+

``` source
@MainActor
var titlebarAppearsTransparent: Bool { get set }
```

## Discussion

When the value of this property is true, the title bar does not draw its background, which allows all content underneath it to show through. It only makes sense to set this property to true when NSFullSizeContentViewWindowMask is also set.

## See Also

### Managing Title Bars

class func standardWindowButton(NSWindow.ButtonType, for: NSWindow.StyleMask) -> NSButton?

Returns a new instance of a given standard window button, sized appropriately for a given window style.

func standardWindowButton(NSWindow.ButtonType) -> NSButton?

Returns the window button of a given window button kind in the window’s view hierarchy.

var showsToolbarButton: Bool

A Boolean value that indicates whether the toolbar control button is currently displayed.

Deprecated

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


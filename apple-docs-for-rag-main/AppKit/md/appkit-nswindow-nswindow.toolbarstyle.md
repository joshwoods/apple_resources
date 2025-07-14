

- AppKit
- NSWindow
-  NSWindow.ToolbarStyle 

Enumeration

# NSWindow.ToolbarStyle

Styles that determine the appearance and location of the toolbar in relation to the title bar.

macOS 11.0+

``` source
enum ToolbarStyle
```

## Topics

### Styles

case automatic

A style indicating that the system determines the toolbar’s appearance and location.

case expanded

A style indicating that the toolbar appears below the window title.

case preference

A style indicating that the toolbar appears below the window title with toolbar items centered in the toolbar.

case unified

A style indicating that the toolbar appears next to the window title.

case unifiedCompact

A style indicating that the toolbar appears next to the window title and with reduced margins to allow more focus on the window’s contents.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var titlebarSeparatorStyle: NSTitlebarSeparatorStyle

The type of separator that the app displays between the title bar and content of a window.

enum NSTitlebarSeparatorStyle

Styles that determine the type of separator displayed between the title bar and content of a window.

var windowTitlebarLayoutDirection: NSUserInterfaceLayoutDirection

The direction the window’s title bar lays text out, either left to right or right to left.




- AppKit
- NSWindow
-  standardWindowButton(\_:for:) 

Type Method

# standardWindowButton(\_:for:)

Returns a new instance of a given standard window button, sized appropriately for a given window style.

macOS

``` source
@MainActor
class func standardWindowButton(
    _ b: NSWindow.ButtonType,
    for styleMask: NSWindow.StyleMask
) -> NSButton?
```

## Parameters 

`b`  

The type of standard window button to return.

`styleMask`  

The window style for which `b` is to be sized. See NSWindow.StyleMask for the list of allowable values.

## Return Value

The new window button of the type identified by `b`; `nil` when no such button type exists.

## Discussion

The caller is responsible for adding the button to the view hierarchy and for setting the target to be the window.

## See Also

### Managing Title Bars

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

var windowTitlebarLayoutDirection: NSUserInterfaceLayoutDirection

The direction the window’s title bar lays text out, either left to right or right to left.


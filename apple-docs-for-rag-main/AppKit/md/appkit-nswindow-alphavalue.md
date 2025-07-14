

- AppKit
- NSWindow
-  alphaValue 

Instance Property

# alphaValue

The window’s alpha value.

macOS

``` source
@MainActor
var alphaValue: CGFloat { get set }
```

## See Also

### Configuring the Window’s Appearance

var styleMask: NSWindow.StyleMask

Flags that describe the window’s current style, such as if it’s resizable or in full-screen mode.

struct StyleMask

Constants that specify the style of a window, and that you can combine with the C bitwise OR operator.

func toggleFullScreen(Any?)

Takes the window into or out of fullscreen mode,

var worksWhenModal: Bool

A Boolean value that indicates whether the window is able to receive keyboard and mouse events even when some other window is being run modally.

var backgroundColor: NSColor!

The color of the window’s background.

var colorSpace: NSColorSpace?

The window’s color space.

func setDynamicDepthLimit(Bool)

Sets a Boolean value that indicates whether the window’s depth limit can change to match the depth of the screen it’s on.

var canHide: Bool

A Boolean value that indicates whether the window can hide when its application becomes hidden.

var isOnActiveSpace: Bool

A Boolean value that indicates whether the window is on the currently active space.

var hidesOnDeactivate: Bool

A Boolean value that indicates whether the window is removed from the screen when its application becomes inactive.

var collectionBehavior: NSWindow.CollectionBehavior

A value that identifies the window’s behavior in window collections.

var isOpaque: Bool

A Boolean value that indicates whether the window is opaque.

var hasShadow: Bool

A Boolean value that indicates whether the window has a shadow.

func invalidateShadow()

Invalidates the window shadow so that it is recomputed based on the current window shape.

func autorecalculatesContentBorderThickness(for: NSRectEdge) -> Bool

Indicates whether the window calculates the thickness of a given border automatically.


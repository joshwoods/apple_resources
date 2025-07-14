

- AppKit
- NSWindow
-  preventsApplicationTerminationWhenModal 

Instance Property

# preventsApplicationTerminationWhenModal

A Boolean value that indicates whether the window prevents application termination when modal.

macOS 10.6+

``` source
@MainActor
var preventsApplicationTerminationWhenModal: Bool { get set }
```

## Discussion

The value of this property is true if the window prevents application termination when modal; otherwise, false. The default value is true.

Usually, application termination is prevented when a modal window or sheet is open, without consulting the application delegate. Some windows may wish not to prevent termination, however. Setting this property to false overrides the default behavior and allows termination to proceed even if the window is open, either through the sudden termination path if enabled, or after consulting the application delegate.

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

var alphaValue: CGFloat

The window’s alpha value.

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


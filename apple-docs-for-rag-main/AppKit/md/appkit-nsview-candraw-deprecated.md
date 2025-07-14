

- AppKit
- NSView
-  canDraw Deprecated

Instance Property

# canDraw

A Boolean value indicating whether drawing commands will produce any results.

macOS 10.0–10.14Deprecated

``` source
@MainActor
var canDraw: Bool { get }
```

Deprecated

If a view needs display, -drawRect: or -updateLayer will be called automatically when the view is able to draw. To check whether a view is in a window, call -window. To check whether a view is hidden, call -isHiddenOrHasHiddenAncestor.

## Discussion

The value of this property is true when drawing produces expected results. A view object can draw onscreen if it is not hidden, it is attached to a view hierarchy in a window (NSWindow), and the window has a corresponding window device. A view object can also draw during printing if it is a descendant of the view being printed.

Check the value of this property before attempting to force drawing to a specific context. For example, if the value of this property is false, do not call lockFocus() or do issue any drawing commands from the view. You do not need to check whether drawing can occur when calling the display() method or any of its related methods. The display methods perform appropriate checks before asking the view to draw itself.

## See Also

### Related Documentation

var isHidden: Bool

A Boolean value indicating whether the view is hidden.

### Properties

var wantsExtendedDynamicRangeOpenGLSurface: BoolDeprecated

var acceptsTouchEvents: Bool

A Boolean value indicating whether the view accepts touch events.

Deprecated

var wantsBestResolutionOpenGLSurface: Bool

A Boolean value indicating whether the view wants an OpenGL backing surface with a resolution greater than 1 pixel per point.

Deprecated




- AppKit
- NSView
-  wantsBestResolutionOpenGLSurface Deprecated

Instance Property

# wantsBestResolutionOpenGLSurface

A Boolean value indicating whether the view wants an OpenGL backing surface with a resolution greater than 1 pixel per point.

macOS 10.7–10.14Deprecated

``` source
@MainActor
var wantsBestResolutionOpenGLSurface: Bool { get set }
```

Deprecated

Use NSOpenGLView instead.

## Return Value

true if the view wants a high resolution backing surface or false if it does not.

## Discussion

This property is relevant only for views bound to an NSOpenGLContext object (including, but not limited to, NSOpenGLView objects). Layer-backed views ignore the value in this property and configure their own backing surface at an appropriate resolution.

Important

For applications linked on macOS 10.15 or later, the default value of this property is true. For applications linked on macOS 10.14 or earlier, the default value of this property is false to keep binary compatibility.

When this property is false, the view uses a 1 pixel per point framebuffer regardless of the backing scale factor for the targeted display. When the backing scale factor is greater than `1.0`, the rendered surface contents are also magnified to the appropriate user size.

When this property is true, AppKit has permission to allocate a higher resolution frame buffer for the view. AppKit uses the backing scale factor and the targeted display to determine whether a higher resolution buffer is appropriate, and it may change the surface resolution when the display mode changes or the view moves to a different display. The view must be able to convert between view units and pixel units when needed. For example, passing the view’s bounds unmodified to the `glViewport` function yields incorrect results at backing scale factors other than `1.0`. You can use the convertToBacking(_:), convertToBacking(_:), and convertToBacking(_:) methods to convert coordinate values to the resolution of the backing store.

To learn more about using OpenGL in your Mac app, see OpenGL Programming Guide for Mac.

## See Also

### Properties

var wantsExtendedDynamicRangeOpenGLSurface: BoolDeprecated

var acceptsTouchEvents: Bool

A Boolean value indicating whether the view accepts touch events.

Deprecated

var canDraw: Bool

A Boolean value indicating whether drawing commands will produce any results.

Deprecated


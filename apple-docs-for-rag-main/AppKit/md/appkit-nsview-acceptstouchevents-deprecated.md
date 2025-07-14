

- AppKit
- NSView
-  acceptsTouchEvents Deprecated

Instance Property

# acceptsTouchEvents

A Boolean value indicating whether the view accepts touch events.

macOS 10.6–10.12.2Deprecated

``` source
@MainActor
var acceptsTouchEvents: Bool { get set }
```

Deprecated

Use allowedTouchTypes instead.

## Discussion

A view accepts touch events when the value of this property is true. By default, views do not accept touch events, so the default value of this property is false. You can override this property and return a different value if you want your view to handle touch events.

## See Also

### Properties

var wantsExtendedDynamicRangeOpenGLSurface: BoolDeprecated

var canDraw: Bool

A Boolean value indicating whether drawing commands will produce any results.

Deprecated

var wantsBestResolutionOpenGLSurface: Bool

A Boolean value indicating whether the view wants an OpenGL backing surface with a resolution greater than 1 pixel per point.

Deprecated


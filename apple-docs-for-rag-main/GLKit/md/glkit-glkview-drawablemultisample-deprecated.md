

- GLKit
- GLKView
-  drawableMultisample Deprecated

Instance Property

# drawableMultisample

The format of the multisampling buffer.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
@MainActor
var drawableMultisample: GLKViewDrawableMultisample { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

The default value is GLKViewDrawableMultisample.multisampleNone.

After your application changes the value of this property, the view recreates its framebuffer object the next time the view is drawn.

## See Also

### Configuring the Framebuffer Object

var drawableColorFormat: GLKViewDrawableColorFormat

The format of the color renderbuffer.

Deprecated

var drawableDepthFormat: GLKViewDrawableDepthFormat

The format of the depth renderbuffer

Deprecated

var drawableStencilFormat: GLKViewDrawableStencilFormat

The format of the stencil renderbuffer.

Deprecated


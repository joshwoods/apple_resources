

- GLKit
- GLKView
-  enableSetNeedsDisplay Deprecated

Instance Property

# enableSetNeedsDisplay

A Boolean value that indicates whether the view responds to messages that invalidate the view’s contents.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
@MainActor
var enableSetNeedsDisplay: Bool { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

By default, a `GLKView` object respects the standard view drawing cycle for a UIView object. However, many OpenGL ES applications need to update their contents explicitly in an animation rendering loop. When updating your contents in a rendering loop, the normal on-demand mechanism for view updates can be disabled by setting the value of this property to false. If your application uses a GLKViewController object to drive the rendering loop, the view controller automatically sets this property to false.

## See Also

### Drawing Your View’s Contents

var context: EAGLContext

The OpenGL ES context used when drawing the view’s contents.

Deprecated

func bindDrawable()

Binds the underlying framebuffer object to OpenGL ES.

Deprecated

func display()

Redraws the view’s contents immediately.

Deprecated

var snapshot: UIImage

Draws the contents of the view and returns them as a new image object.

Deprecated


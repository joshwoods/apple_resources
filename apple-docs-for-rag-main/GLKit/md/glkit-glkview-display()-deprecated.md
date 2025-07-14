

- GLKit
- GLKView
-  display() Deprecated

Instance Method

# display()

Redraws the view’s contents immediately.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
@MainActor
func display()
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

This method causes your drawing method to be called immediately and then presents the rendered image to the screen. Your application typically calls this method inside of a rendering loop, such as the one provided by the GLKViewController class, in order to provide a continuous smooth animation.

Never call this method inside your drawing function.

## See Also

### Drawing Your View’s Contents

var context: EAGLContext

The OpenGL ES context used when drawing the view’s contents.

Deprecated

func bindDrawable()

Binds the underlying framebuffer object to OpenGL ES.

Deprecated

var enableSetNeedsDisplay: Bool

A Boolean value that indicates whether the view responds to messages that invalidate the view’s contents.

Deprecated

var snapshot: UIImage

Draws the contents of the view and returns them as a new image object.

Deprecated


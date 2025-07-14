

- GLKit
- GLKView
-  bindDrawable() Deprecated

Instance Method

# bindDrawable()

Binds the underlying framebuffer object to OpenGL ES.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
@MainActor
func bindDrawable()
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

Before calling your drawing method, the view binds the underlying framebuffer object to the context so that rendering commands are automatically drawn into it. However, some rendering strategies require you to change the target of your rendering commands to another framebuffer object, such as when you need to render to a texture first. If your application changed the framebuffer object bound to OpenGL ES, it calls this method to rebind the view’s framebuffer object to OpenGL ES.

## See Also

### Drawing Your View’s Contents

var context: EAGLContext

The OpenGL ES context used when drawing the view’s contents.

Deprecated

var enableSetNeedsDisplay: Bool

A Boolean value that indicates whether the view responds to messages that invalidate the view’s contents.

Deprecated

func display()

Redraws the view’s contents immediately.

Deprecated

var snapshot: UIImage

Draws the contents of the view and returns them as a new image object.

Deprecated


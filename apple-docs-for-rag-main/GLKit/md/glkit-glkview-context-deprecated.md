

- GLKit
- GLKView
-  context Deprecated

Instance Property

# context

The OpenGL ES context used when drawing the view’s contents.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
@MainActor
var context: EAGLContext { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

The view uses this context as the place to create its underlying framebuffer object and it also sets the context before calling your drawing method. Never change the context from inside your drawing method.

## See Also

### Drawing Your View’s Contents

func bindDrawable()

Binds the underlying framebuffer object to OpenGL ES.

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


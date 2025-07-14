

- GLKit
- GLKView
-  snapshot Deprecated

Instance Property

# snapshot

Draws the contents of the view and returns them as a new image object.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
@MainActor
var snapshot: UIImage { get }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Return Value

An image object.

## Discussion

When this method is called, the view sets up a drawing environment and calls your drawing method. However, instead of presenting the view’s contents on screen, they are returned to your application as an image instead. This method should be called whenever your application explicitly needs the contents of the view; never attempt to directly read the contents of the underlying framebuffer using OpenGL ES functions.

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

func display()

Redraws the view’s contents immediately.

Deprecated


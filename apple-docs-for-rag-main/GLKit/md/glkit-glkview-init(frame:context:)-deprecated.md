

- GLKit
- GLKView
-  init(frame:context:) Deprecated

Initializer

# init(frame:context:)

Initializes a new view.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
@MainActor
init(
    frame: CGRect,
    context: EAGLContext
)
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`frame`  

The frame rectangle for the view, measured in points. The origin of the frame is relative to the superview in which you plan to add it. This method uses the frame rectangle to set thecenter and bounds properties accordingly.

`context`  

An OpenGL ES context used to store the framebuffer object.

## Return Value

An initialized view object or `nil` if the object couldn’t be created.


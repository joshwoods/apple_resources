

- Quartz
- QCRenderer
-  render(atTime:arguments:) Deprecated

Instance Method

# render(atTime:arguments:)

Renders a frame of a composition at the specified time.

macOS 10.4–10.15Deprecated

``` source
func render(
    atTime time: TimeInterval,
    arguments: [AnyHashable : Any]!
) -> Bool
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`time`  

The time, in seconds, at which to render a composition frame. The time must be a positive value or zero.

`arguments`  

An optional dictionary that can have any of the entries defined in Rendering Arguments.

## Return Value

true if successful.

## Discussion

You need to call this method each time you want to render a frame of the composition.

All OpenGL states are preserved *except* the following:

- States defined by `GL_CURRENT_BIT`

- Textures on each unit and the environment mode

- Matrix mode

If you are using double buffers, keep in mind that the `renderAtTime:arguments:` method does not swap the front and back buffers of the OpenGL context. You must perform the swap yourself by calling the OpenGL command `flushBuffer` on the context associated with the renderer.

If you are interleaving OpenGL code with rendering of a composition, make sure that the OpenGL context is current. If you are using the NSOpenGLContext class, call the makeCurrentContext() method prior to rendering. If you are using the CGL API, call the function `CGLSetCurrentContext(_:)`.


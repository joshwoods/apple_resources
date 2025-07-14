

- Compositor Services
- LayerRenderer
-  queryNextFrame() 

Instance Method

# queryNextFrame()

Returns the next frame to use for drawing.

visionOS 1.0+

``` source
func queryNextFrame() -> LayerRenderer.Frame?
```

## Return Value

A frame type to use for drawing operations. The function returns `nil` if the layer is paused, invalidated, or has too many frames already in use.

## Mentioned in 

Drawing fully immersive content using Metal

## Discussion

This function retrieves the next frame for you to use in your drawing operations. The system maintains a limited number of frames, so don’t try to render more than one frame in advance. If this function returns `nil`, wait a short time and try again. When the system finishes displaying a rendered frame, it returns that frame to the shared pool and makes it available for you to use again.

The index of each returned frame is always greater than the index of the previous frame. The system increments index values sequentially so you can differentiate frames you are currently drawing.

## See Also

### Drawing a frame of content

struct Frame

A type that provides access to the timing information and data types you need to render a single frame of content.

struct Drawable

A type that provides the textures and information you need to draw a frame of content.


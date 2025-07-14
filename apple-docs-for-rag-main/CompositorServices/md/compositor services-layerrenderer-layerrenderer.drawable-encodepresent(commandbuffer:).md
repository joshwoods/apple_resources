

- Compositor Services
- LayerRenderer
- LayerRenderer.Drawable
-  encodePresent(commandBuffer:) 

Instance Method

# encodePresent(commandBuffer:)

Encodes a notification event to the specified command buffer to present the drawable’s content onscreen.

visionOS 1.0+

``` source
func encodePresent(commandBuffer command_buffer: any MTLCommandBuffer)
```

## Parameters 

`command_buffer`  

The command buffer you used to encode your frame’s content. If the command buffer is already committed, this function aborts your app with an error.

## Mentioned in 

Drawing fully immersive content using Metal

## Discussion

Call this function as the last step before committing the specified command buffer. Specifically, call it after you finish encoding all the work required to render the frame, and immediately before you call the command buffer’s commit() method. The function adds a presentation event to the buffer that causes the compositor to display your frame.


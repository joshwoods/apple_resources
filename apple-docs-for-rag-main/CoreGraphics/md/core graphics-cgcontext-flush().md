

- Core Graphics
- CGContext
-  flush() 

Instance Method

# flush()

Forces all pending drawing operations in a window context to be rendered immediately to the destination device.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func flush()
```

## Discussion

When you call this function, Core Graphics immediately flushes the current drawing to the destination device (for example, a screen). Because the system software flushes a context automatically at the appropriate times, calling this function could have an adverse effect on performance. Under normal conditions, you do not need to call this function.

## See Also

### Managing a Graphics Context

func synchronize()

Marks a window context for update.

func setBlendMode(CGBlendMode)

Sets how sample values are composited by a graphics context.

enum CGBlendMode

Compositing operations for images.

func setRenderingIntent(CGColorRenderingIntent)

Sets the rendering intent in the current graphics state.


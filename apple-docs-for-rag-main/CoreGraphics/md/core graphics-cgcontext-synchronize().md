

- Core Graphics
- CGContext
-  synchronize() 

Instance Method

# synchronize()

Marks a window context for update.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func synchronize()
```

## Discussion

When you call this function, all drawing operations since the last update are flushed at the next regular opportunity. Under normal conditions, you do not need to call this function.

## See Also

### Managing a Graphics Context

func flush()

Forces all pending drawing operations in a window context to be rendered immediately to the destination device.

func setBlendMode(CGBlendMode)

Sets how sample values are composited by a graphics context.

enum CGBlendMode

Compositing operations for images.

func setRenderingIntent(CGColorRenderingIntent)

Sets the rendering intent in the current graphics state.


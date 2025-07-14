

- Core Graphics
- CGContext
-  setBlendMode(\_:) 

Instance Method

# setBlendMode(\_:)

Sets how sample values are composited by a graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setBlendMode(_ mode: CGBlendMode)
```

## Parameters 

`mode`  

A blend mode. See CGBlendMode for a list of the constants you can supply.

## See Also

### Managing a Graphics Context

func flush()

Forces all pending drawing operations in a window context to be rendered immediately to the destination device.

func synchronize()

Marks a window context for update.

enum CGBlendMode

Compositing operations for images.

func setRenderingIntent(CGColorRenderingIntent)

Sets the rendering intent in the current graphics state.


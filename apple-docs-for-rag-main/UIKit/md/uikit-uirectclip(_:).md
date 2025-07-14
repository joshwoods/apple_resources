

- UIKit
-  UIRectClip(\_:) 

Function

# UIRectClip(\_:)

Modifies the current clipping path by intersecting it with the specified rectangle.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
func UIRectClip(_ rect: CGRect)
```

## Parameters 

`rect`  

The rectangle to intersect with the clipping region. If the width or height of the rectangle are less than 0, this function does not change the clipping path.

## Discussion

Each call to this function permanently shrinks the clipping path of the current graphics context using the specified rectangle. You cannot use this function to expand the clipping region path. If the current graphics context is `nil`, this function does nothing.

If you need to return the clipping path to its original shape in your drawing code, you should save the current graphics context before calling this function. To save the current state of the graphics context, call the saveGState() function before making your modifications. When you are ready to restore the original clipping region, you can then use the restoreGState() function to restore the previous graphics state.

This function may be called from any thread of your app.

## See Also

### Graphics context primitives

func UIGraphicsGetCurrentContext() -> CGContext?

Returns the current graphics context.

func UIGraphicsPushContext(CGContext)

Makes the specified graphics context the current context.

func UIGraphicsPopContext()

Removes the current graphics context from the top of the stack, restoring the previous context.

func UIGraphicsBeginImageContextWithOptions(CGSize, Bool, CGFloat)

Creates a bitmap-based graphics context with the specified options.

Deprecated


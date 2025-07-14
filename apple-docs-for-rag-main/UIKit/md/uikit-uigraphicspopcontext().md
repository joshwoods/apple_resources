

- UIKit
-  UIGraphicsPopContext() 

Function

# UIGraphicsPopContext()

Removes the current graphics context from the top of the stack, restoring the previous context.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
func UIGraphicsPopContext()
```

## Discussion

Use this function to balance calls to the UIGraphicsPushContext(_:) function.

This function may be called from any thread of your app.

## See Also

### Graphics context primitives

func UIGraphicsGetCurrentContext() -> CGContext?

Returns the current graphics context.

func UIGraphicsPushContext(CGContext)

Makes the specified graphics context the current context.

func UIGraphicsBeginImageContextWithOptions(CGSize, Bool, CGFloat)

Creates a bitmap-based graphics context with the specified options.

Deprecated

func UIRectClip(CGRect)

Modifies the current clipping path by intersecting it with the specified rectangle.


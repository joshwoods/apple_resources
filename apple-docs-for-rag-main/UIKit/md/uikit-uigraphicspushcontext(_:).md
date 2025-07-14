

- UIKit
-  UIGraphicsPushContext(\_:) 

Function

# UIGraphicsPushContext(\_:)

Makes the specified graphics context the current context.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
func UIGraphicsPushContext(_ context: CGContext)
```

## Parameters 

`context`  

The graphics context to make the current context.

## Discussion

You can use this function to save the previous graphics state and make the specified context the current context. You must balance calls to this function with matching calls to the UIGraphicsPopContext() function.

This function may be called from any thread of your app.

## See Also

### Graphics context primitives

func UIGraphicsGetCurrentContext() -> CGContext?

Returns the current graphics context.

func UIGraphicsPopContext()

Removes the current graphics context from the top of the stack, restoring the previous context.

func UIGraphicsBeginImageContextWithOptions(CGSize, Bool, CGFloat)

Creates a bitmap-based graphics context with the specified options.

Deprecated

func UIRectClip(CGRect)

Modifies the current clipping path by intersecting it with the specified rectangle.


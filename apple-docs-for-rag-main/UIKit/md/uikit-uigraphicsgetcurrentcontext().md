

- UIKit
-  UIGraphicsGetCurrentContext() 

Function

# UIGraphicsGetCurrentContext()

Returns the current graphics context.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
func UIGraphicsGetCurrentContext() -> CGContext?
```

## Return Value

The current graphics context.

## Discussion

The current graphics context is `nil` by default. Prior to calling its `drawRect:` method, view objects push a valid context onto the stack, making it current. If you are not using a `UIView` object to do your drawing, however, you must push a valid context onto the stack manually using the UIGraphicsPushContext(_:) function.

This function may be called from any thread of your app.

## See Also

### Graphics context primitives

func UIGraphicsPushContext(CGContext)

Makes the specified graphics context the current context.

func UIGraphicsPopContext()

Removes the current graphics context from the top of the stack, restoring the previous context.

func UIGraphicsBeginImageContextWithOptions(CGSize, Bool, CGFloat)

Creates a bitmap-based graphics context with the specified options.

Deprecated

func UIRectClip(CGRect)

Modifies the current clipping path by intersecting it with the specified rectangle.


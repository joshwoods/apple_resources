

- UIKit
-  UIGraphicsBeginImageContextWithOptions(\_:\_:\_:) 

Function

# UIGraphicsBeginImageContextWithOptions(\_:\_:\_:)

Creates a bitmap-based graphics context with the specified options.

iOS 4.0–18.4DeprecatediPadOS 4.0–18.4DeprecatedMac Catalyst 13.1+tvOSvisionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
func UIGraphicsBeginImageContextWithOptions(
    _ size: CGSize,
    _ opaque: Bool,
    _ scale: CGFloat
)
```

## Parameters 

`size`  

The size (measured in points) of the new bitmap context. This represents the size of the image returned by the UIGraphicsGetImageFromCurrentImageContext() function. To get the size of the bitmap in pixels, you must multiply the width and height values by the value in the `scale` parameter.

`opaque`  

A Boolean flag indicating whether the bitmap is opaque. If you know the bitmap is fully opaque, specify true to ignore the alpha channel and optimize the bitmap’s storage. Specifying false means that the bitmap must include an alpha channel to handle any partially transparent pixels.

`scale`  

The scale factor to apply to the bitmap. If you specify a value of `0.0`, the scale factor is set to the scale factor of the device’s main screen.

## Discussion

You use this function to configure the drawing environment for rendering into a bitmap. The format for the bitmap is a ARGB 32-bit integer pixel format using host-byte order. If the opaque parameter is true, the alpha channel is ignored and the bitmap is treated as fully opaque (CGImageAlphaInfo.noneSkipFirst \| kCGBitmapByteOrder32Host). Otherwise, each pixel uses a premultipled ARGB format (CGImageAlphaInfo.premultipliedFirst \| kCGBitmapByteOrder32Host).

The environment also uses the default coordinate system for UIKit views, where the origin is in the upper-left corner and the positive axes extend down and to the right of the origin. The supplied scale factor is also applied to the coordinate system and resulting images. The drawing environment is pushed onto the graphics context stack immediately.

While the context created by this function is the current context, you can call the UIGraphicsGetImageFromCurrentImageContext() function to retrieve an image object based on the current contents of the context. When you are done modifying the context, you must call the UIGraphicsEndImageContext() function to clean up the bitmap drawing environment and remove the graphics context from the top of the context stack. You should not use the UIGraphicsPopContext() function to remove this type of context from the stack.

In most other respects, the graphics context created by this function behaves like any other graphics context. You can change the context by pushing and popping other graphics contexts. You can also get the bitmap context using the UIGraphicsGetCurrentContext() function.

This function may be called from any thread of your app.

## See Also

### Related Documentation

func UIGraphicsEndImageContext()

Removes the current bitmap-based graphics context from the top of the stack.

Deprecated

func UIGraphicsGetImageFromCurrentImageContext() -> UIImage?

Returns an image from the contents of the current bitmap-based graphics context.

Deprecated

### Graphics context primitives

func UIGraphicsGetCurrentContext() -> CGContext?

Returns the current graphics context.

func UIGraphicsPushContext(CGContext)

Makes the specified graphics context the current context.

func UIGraphicsPopContext()

Removes the current graphics context from the top of the stack, restoring the previous context.

func UIRectClip(CGRect)

Modifies the current clipping path by intersecting it with the specified rectangle.


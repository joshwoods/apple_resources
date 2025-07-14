

- UIKit
- UIGraphicsRendererContext
-  clip(to:) 

Instance Method

# clip(to:)

Sets the clipping mask for the drawing context to the specified rectangle.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
func clip(to rect: CGRect)
```

## Parameters 

`rect`  

The rectangle to which the drawing context is clipped, specified in the Core Graphics coordinate space with values in points.

## Discussion

To restrict the active drawing area to the specified rectangle, call this method before executing drawing commands.

To use a more complex shape as a clipping mask, use the clip(to:mask:) method on the underlying Core Graphics context, accessed through the cgContext property.


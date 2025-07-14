

- UIKit
- UIGraphicsRendererContext
-  fill(\_:blendMode:) 

Instance Method

# fill(\_:blendMode:)

Paints a rectangular area with the currently selected fill color using the supplied blend mode.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
func fill(
    _ rect: CGRect,
    blendMode: CGBlendMode
)
```

## Parameters 

`rect`  

A rectangle, specified in the Core Graphics coordinate space with values in points.

`blendMode`  

The blend mode applied to the fill operation.

## Discussion

Before calling this method, select the fill color with the setFill() method on an instance of UIColor.

The blend mode specifies how the new value for a given pixel is calculated, given the existing pixel value and the currently selected fill color. For more information on the blend modes available, see CGBlendMode.

For an example of how to use this method, see Using blend mode in UIGraphicsImageRenderer.

## See Also

### Drawing content

func stroke(CGRect)

Paints a rectangular path using the currently selected stroke color.

func stroke(CGRect, blendMode: CGBlendMode)

Paints a rectangular path using the currently selected stroke color and specified blend mode.

func fill(CGRect)

Paints a rectangular area with the currently selected fill color.


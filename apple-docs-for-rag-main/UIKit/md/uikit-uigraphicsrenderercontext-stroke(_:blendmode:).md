

- UIKit
- UIGraphicsRendererContext
-  stroke(\_:blendMode:) 

Instance Method

# stroke(\_:blendMode:)

Paints a rectangular path using the currently selected stroke color and specified blend mode.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
func stroke(
    _ rect: CGRect,
    blendMode: CGBlendMode
)
```

## Parameters 

`rect`  

A rectangle, specified in the Core Graphics coordinate space with values in points.

`blendMode`  

The blend mode applied to the stroke operation.

## Discussion

Before calling this method, select the stroke color with the setStroke() method on an instance of UIColor.

The blend mode specifies how the new value for a given pixel is calculated, given the existing pixel value and the currently selected fill color. For more information on the blend modes available, see CGBlendMode.

## See Also

### Drawing content

func stroke(CGRect)

Paints a rectangular path using the currently selected stroke color.

func fill(CGRect, blendMode: CGBlendMode)

Paints a rectangular area with the currently selected fill color using the supplied blend mode.

func fill(CGRect)

Paints a rectangular area with the currently selected fill color.


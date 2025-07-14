

- UIKit
- UIGraphicsRendererContext
-  stroke(\_:) 

Instance Method

# stroke(\_:)

Paints a rectangular path using the currently selected stroke color.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
func stroke(_ rect: CGRect)
```

## Parameters 

`rect`  

A rectangle, specified in the Core Graphics coordinate space with values in points.

## Discussion

Before calling this method, select the stroke color with the setStroke() method on an instance of UIColor.

For an example of how to use this method, see Creating an image with an image renderer in UIGraphicsImageRenderer.

## See Also

### Drawing content

func stroke(CGRect, blendMode: CGBlendMode)

Paints a rectangular path using the currently selected stroke color and specified blend mode.

func fill(CGRect, blendMode: CGBlendMode)

Paints a rectangular area with the currently selected fill color using the supplied blend mode.

func fill(CGRect)

Paints a rectangular area with the currently selected fill color.


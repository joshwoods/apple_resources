

- Vision
- DetectRectanglesRequest
-  minimumConfidence 

Instance Property

# minimumConfidence

The minimum acceptable confidence level for detected rectangles.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var minimumConfidence: Float
```

## Discussion

The framework won’t return rectangles with a confidence score lower than the specified minimum.

The confidence score ranges from `0.0` to `1.0`, inclusive, where `0.0` represents no confidence, and `1.0` represents full confidence. The default minimum confidence is `0.0`.

## See Also

### Inspecting a request

var maximumAspectRatio: Float

The maximum aspect ratio of the rectangle to detect.

var maximumObservations: Int

The maximum number of rectangles Vision returns.

var minimumAspectRatio: Float

The minimum aspect ratio of the rectangle(s) to detect.

var minimumSize: Float

The minimum size of the rectangle to be detected, as a proportion of the smallest dimension.

var quadratureToleranceDegrees: Float

The maximum number of degrees a rectangle corner angle can deviate from 90°.


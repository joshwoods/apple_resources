

- Vision
- DetectRectanglesRequest
-  minimumSize 

Instance Property

# minimumSize

The minimum size of the rectangle to be detected, as a proportion of the smallest dimension.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var minimumSize: Float
```

## Discussion

The value should range from `0.0` to `1.0` inclusive. The default minimum size is `0.2`.

Any smaller rectangles that the framework might detect aren’t returned.

## See Also

### Inspecting a request

var maximumAspectRatio: Float

The maximum aspect ratio of the rectangle to detect.

var maximumObservations: Int

The maximum number of rectangles Vision returns.

var minimumAspectRatio: Float

The minimum aspect ratio of the rectangle(s) to detect.

var minimumConfidence: Float

The minimum acceptable confidence level for detected rectangles.

var quadratureToleranceDegrees: Float

The maximum number of degrees a rectangle corner angle can deviate from 90°.


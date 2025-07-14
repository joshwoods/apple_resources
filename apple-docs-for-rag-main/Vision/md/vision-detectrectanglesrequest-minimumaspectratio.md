

- Vision
- DetectRectanglesRequest
-  minimumAspectRatio 

Instance Property

# minimumAspectRatio

The minimum aspect ratio of the rectangle(s) to detect.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var minimumAspectRatio: Float
```

## Discussion

The value should range from `0.0` to `1.0`, inclusive. The default value is `0.5`.

## See Also

### Inspecting a request

var maximumAspectRatio: Float

The maximum aspect ratio of the rectangle to detect.

var maximumObservations: Int

The maximum number of rectangles Vision returns.

var minimumConfidence: Float

The minimum acceptable confidence level for detected rectangles.

var minimumSize: Float

The minimum size of the rectangle to be detected, as a proportion of the smallest dimension.

var quadratureToleranceDegrees: Float

The maximum number of degrees a rectangle corner angle can deviate from 90°.


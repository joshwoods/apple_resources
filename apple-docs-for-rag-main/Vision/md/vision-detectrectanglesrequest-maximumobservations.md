

- Vision
- DetectRectanglesRequest
-  maximumObservations 

Instance Property

# maximumObservations

The maximum number of rectangles Vision returns.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var maximumObservations: Int
```

## Discussion

The default is `1`. Setting this property to `0` allows for returning a potentially unlimited number of observations.

## See Also

### Inspecting a request

var maximumAspectRatio: Float

The maximum aspect ratio of the rectangle to detect.

var minimumAspectRatio: Float

The minimum aspect ratio of the rectangle(s) to detect.

var minimumConfidence: Float

The minimum acceptable confidence level for detected rectangles.

var minimumSize: Float

The minimum size of the rectangle to be detected, as a proportion of the smallest dimension.

var quadratureToleranceDegrees: Float

The maximum number of degrees a rectangle corner angle can deviate from 90°.


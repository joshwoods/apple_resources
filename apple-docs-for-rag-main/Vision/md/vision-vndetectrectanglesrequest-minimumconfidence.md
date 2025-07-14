

- Vision
- VNDetectRectanglesRequest
-  minimumConfidence 

Instance Property

# minimumConfidence

A value specifying the minimum acceptable confidence level.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var minimumConfidence: VNConfidence { get set }
```

## Discussion

Vision won’t return rectangles with a confidence score lower than the specified minimum.

The confidence score ranges from `0.0` to `1.0`, inclusive, where `0.0` represents no confidence, and `1.0` represents full confidence.

## See Also

### Configuring Detection

var minimumAspectRatio: VNAspectRatio

A `float` specifying the minimum aspect ratio of the rectangle to detect, defined as the shorter dimension over the longer dimension.

var maximumAspectRatio: VNAspectRatio

A `float` specifying the maximum aspect ratio of the rectangle to detect, defined as the shorter dimension over the longer dimension.

typealias VNAspectRatio

A type alias for expressing rectangle aspect ratios in Vision.

var quadratureTolerance: VNDegrees

A float specifying the number of degrees a rectangle corner angle can deviate from 90°.

typealias VNDegrees

A typealias for expressing tolerance angles in Vision.

var minimumSize: Float

The minimum size of a rectangle to detect, as a proportion of the smallest dimension.

typealias VNConfidence

A type alias for the confidence value of an observation.

var maximumObservations: Int

An integer specifying the maximum number of rectangles Vision returns.




- Vision
-  VNConfidence 

Type Alias

# VNConfidence

A type alias for the confidence value of an observation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
typealias VNConfidence = Float
```

## Discussion

The Vision framework normalizes this value to `[0.0, 1.0]` under most circumstances. A value of `0.0` indicates no confidence. A value of `1.0` indicates highest confidence, or the observation doesn’t support or assign meaning to confidence.

Note

When the results come from a VNCoreMLRequest, Vision forwards confidence values as-is and doesn’t normalize them.

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

var minimumConfidence: VNConfidence

A value specifying the minimum acceptable confidence level.

var maximumObservations: Int

An integer specifying the maximum number of rectangles Vision returns.




- Vision
-  VNAspectRatio 

Type Alias

# VNAspectRatio

A type alias for expressing rectangle aspect ratios in Vision.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
typealias VNAspectRatio = Float
```

## Discussion

The value is a float, but limited to a range of `0.0` to `1.0`, inclusive, with the default of `0.5` indicating a square image. It defines aspect ratio as the shorter dimension over the longer dimension.

## See Also

### Configuring Detection

var minimumAspectRatio: VNAspectRatio

A `float` specifying the minimum aspect ratio of the rectangle to detect, defined as the shorter dimension over the longer dimension.

var maximumAspectRatio: VNAspectRatio

A `float` specifying the maximum aspect ratio of the rectangle to detect, defined as the shorter dimension over the longer dimension.

var quadratureTolerance: VNDegrees

A float specifying the number of degrees a rectangle corner angle can deviate from 90°.

typealias VNDegrees

A typealias for expressing tolerance angles in Vision.

var minimumSize: Float

The minimum size of a rectangle to detect, as a proportion of the smallest dimension.

var minimumConfidence: VNConfidence

A value specifying the minimum acceptable confidence level.

typealias VNConfidence

A type alias for the confidence value of an observation.

var maximumObservations: Int

An integer specifying the maximum number of rectangles Vision returns.


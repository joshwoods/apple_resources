

- Vision
- VNImageAestheticsScoresObservation
-  overallScore 

Instance Property

# overallScore

A score that incorporates the aesthetic score, failure score, and utility labels.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var overallScore: Float { get }
```

## Discussion

This returns a value within the range of `-1` and `1`, where `1` is most desirable and `-1` isn’t desireable.

## See Also

### Parsing Observation Content

var isUtility: Bool

Returns a Boolean value that represents an image that may not have memorable or exciting content.


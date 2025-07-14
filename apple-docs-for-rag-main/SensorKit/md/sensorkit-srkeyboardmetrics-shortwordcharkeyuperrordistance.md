

- SensorKit
- SRKeyboardMetrics
-  shortWordCharKeyUpErrorDistance 

Instance Property

# shortWordCharKeyUpErrorDistance

The distance from the touch up to the center of the intended key of a character in a short word.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var shortWordCharKeyUpErrorDistance: ProbabilityMetric { get }
```

## See Also

### Measuring Key Use

var longWordUpErrorDistance: [ProbabilityMetric&lt;UnitLength>]

The distance from the touch up to the center of the intended key of the characters of a long word.

var longWordDownErrorDistance: [ProbabilityMetric&lt;UnitLength>]

The distance from the touch down to the center of the intended key of the characters of a long word.

var upErrorDistance: ProbabilityMetric&lt;UnitLength>

The distance from the touch up to the center of any key.

var downErrorDistance: ProbabilityMetric&lt;UnitLength>

The distance from the touch down to the center of any key.

var spaceUpErrorDistance: ProbabilityMetric&lt;UnitLength>

The distance from the touch up to the right centroid of the Space bar.

var spaceDownErrorDistance: ProbabilityMetric&lt;UnitLength>

The distance from the touch down to the right centroid of the Space bar.

var deleteUpErrorDistance: ProbabilityMetric&lt;UnitLength>

The distance from the touch up to the center of the Delete key.

var deleteDownErrorDistance: ProbabilityMetric&lt;UnitLength>

The distance from the touch down to the center of the Delete key.

var shortWordCharKeyDownErrorDistance: ProbabilityMetric&lt;UnitLength>

The distance from the touch down to the center of the intended key of a character in a short word.

var pathErrorDistanceRatio: [NSNumber]

Sample values of the ratio of error distance between the intended and actual path.


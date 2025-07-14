

- Exposure Notification
- ENExposureConfiguration
-  minimumRiskScoreFullRange 

Instance Property

# minimumRiskScoreFullRange

The value that is the user’s full-range minimum risk score.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var minimumRiskScoreFullRange: Double { get set }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.6 and later.

The framework excludes exposure incidents with scores lower than the value of this property. There is no default minimum value for this property. This value isn’t limited by ENRiskScore.

The framework doesn’t use this property when calculating matchedKeyCount or daysSinceLastExposure.

## See Also

### Minimum Threshold Configuration

var minimumRiskScore: ENRiskScore

The value that is the user’s minimum risk score.




- Exposure Notification
- ENExposureDetectionSummary
-  daysSinceLastExposure 

Instance Property

# daysSinceLastExposure

Number of days since the most recent exposure.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var daysSinceLastExposure: Int { get }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.5 and later.

The values for this property represent the number of days since the most recent exposure, going backwards. For example, a value of `0` means that the person was exposed today, `1` was yesterday, `2` was two days ago, and so on.

This property is only valid if matchedKeyCount \> 0.

The framework computes this property’s value across all matching exposures, not just exposures that meet or exceed minimumRiskScore or minimumRiskScoreFullRange.

Note

This value is only available when `ENAPIVersion` is set to `1` in the app’s Info.plist file.

## See Also

### Exposure Criteria

var attenuationDurations: [NSNumber]

An array of durations at specific radio signal attenuations.

var matchedKeyCount: UInt64

The number of keys that matched for an exposure detection.

var maximumRiskScore: ENRiskScore

The vaue that represents the highest risk score of all exposure incidents.

var maximumRiskScoreFullRange: Double

The value that represents the highest, full-range risk score of all the exposures for the user.

var riskScoreSumFullRange: Double

The sum of the full-range risk scores for all exposures for the user.

var metadata: [AnyHashable : Any]?

The metadata associated with the summary.

var daySummaries: [ENExposureDaySummary]

The summary of each day that contains an exposure.


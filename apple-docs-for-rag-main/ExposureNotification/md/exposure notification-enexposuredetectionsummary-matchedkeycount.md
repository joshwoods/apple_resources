

- Exposure Notification
- ENExposureDetectionSummary
-  matchedKeyCount 

Instance Property

# matchedKeyCount

The number of keys that matched for an exposure detection.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var matchedKeyCount: UInt64 { get }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.5 and later.

The framework computes this property’s value across all matching exposures, not just exposures that meet or exceed minimumRiskScore or minimumRiskScoreFullRange.

This value is only available when `ENAPIVersion` is set to `1` in the app’s `Info.plist` file.

## See Also

### Exposure Criteria

var attenuationDurations: [NSNumber]

An array of durations at specific radio signal attenuations.

var daysSinceLastExposure: Int

Number of days since the most recent exposure.

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


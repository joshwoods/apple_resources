

- Exposure Notification
- ENExposureDetectionSummary
-  metadata 

Instance Property

# metadata

The metadata associated with the summary.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var metadata: [AnyHashable : Any]? { get }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.5 and later.

Not used.

## See Also

### Exposure Criteria

var attenuationDurations: [NSNumber]

An array of durations at specific radio signal attenuations.

var daysSinceLastExposure: Int

Number of days since the most recent exposure.

var matchedKeyCount: UInt64

The number of keys that matched for an exposure detection.

var maximumRiskScore: ENRiskScore

The vaue that represents the highest risk score of all exposure incidents.

var maximumRiskScoreFullRange: Double

The value that represents the highest, full-range risk score of all the exposures for the user.

var riskScoreSumFullRange: Double

The sum of the full-range risk scores for all exposures for the user.

var daySummaries: [ENExposureDaySummary]

The summary of each day that contains an exposure.


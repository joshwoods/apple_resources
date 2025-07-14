

- Exposure Notification
- ENExposureDetectionSummary
-  attenuationDurations 

Instance Property

# attenuationDurations

An array of durations at specific radio signal attenuations.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var attenuationDurations: [NSNumber] { get }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.5 and later.

An array that contains the duration, in seconds, at certain attenuations, using an aggregated maximum exposures of 30 minutes.

`array[0]` = Sum of durations for all exposures when attenuation value was `A attenuationDurationThresholds to configure the `X` and `Y` values.

Note

This value is only available when `ENAPIVersion` is set to `1` in the app’s Info.plist file.

## See Also

### Exposure Criteria

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

var metadata: [AnyHashable : Any]?

The metadata associated with the summary.

var daySummaries: [ENExposureDaySummary]

The summary of each day that contains an exposure.


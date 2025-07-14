

- Exposure Notification
- ENExposureInfo
-  duration 

Instance Property

# duration

The length of time that the contact was in proximity to the user.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var duration: TimeInterval { get }
```

## Discussion

When reporting the duration of an exposure, the values are stored as seconds rounded up to the next minute. A duration value caps at 30 minutes (1800 seconds).

Note

In iOS 13.5, duration values are rounded up to the next 5-minute interval.

## See Also

### Exposure Criteria

var attenuationDurations: [NSNumber]

An array of durations at specific radio signal attenuations.

var attenuationValue: ENAttenuation

The attenutation risk level value for the exposure.

var date: Date

The date the exposure occurred.

var totalRiskScore: ENRiskScore

The value that represents the total risk score the framework calculates for this exposure incident.

var totalRiskScoreFullRange: Double

The value that represents the full-range total risk score the framework calculates for this exposure incident.

var transmissionRiskLevel: ENRiskLevel

The transmission risk associated with a diagnosis key.

typealias ENAttenuation

The signal strength value.

var metadata: [AnyHashable : Any]?

The metadata associated with the exposure information.

var daysSinceOnsetOfSymptoms: Int

The number of days since the onset of symptoms.

var diagnosisReportType: ENDiagnosisReportType

The method used to report the positive diagnosis.

let ENDaysSinceOnsetOfSymptomsUnknown: Int

A value used when the number of days since onset of symptoms is unknown.

Deprecated


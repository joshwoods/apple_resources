

- Exposure Notification
- ENExposureInfo
-  attenuationValue 

Instance Property

# attenuationValue

The attenutation risk level value for the exposure.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var attenuationValue: ENAttenuation { get }
```

## Discussion

Because attenuation can vary over a specific exposure event, the attenuation risk level value is calculated by weighting attenuation risk level values based on their durations during the exposure event.

The attenuation risk level values are configured with attenuationLevelValues.

## See Also

### Exposure Criteria

var attenuationDurations: [NSNumber]

An array of durations at specific radio signal attenuations.

var date: Date

The date the exposure occurred.

var duration: TimeInterval

The length of time that the contact was in proximity to the user.

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


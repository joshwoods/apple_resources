

- Exposure Notification
-  ENExposureInfo 

Class

# ENExposureInfo

The incident information related to a potential exposure.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
class ENExposureInfo
```

## Overview

Important

This class is available in iOS 12.5, and in iOS 13.5 and later. It isn’t supported for apps with ENAPIVersion set to `2` in the `Info.plist` file. Instead, getExposureWindows(summary:completionHandler:) provides an array of ENExposureWindow objects.

This class carries information about an exposure incident.

## Topics

### Exposure Criteria

var attenuationDurations: [NSNumber]

An array of durations at specific radio signal attenuations.

var attenuationValue: ENAttenuation

The attenutation risk level value for the exposure.

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

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Exposure Information

typealias ENRiskScore

A value signifying the risk of an exposure event.

typealias ENRiskLevel

The user’s estimated risk of exposure.

typealias ENRiskLevelValue

The value associated with a particular risk level.




- Exposure Notification
-  ENExposureConfiguration 

Class

# ENExposureConfiguration

The object that contains parameters for configuring exposure notification risk scoring behavior.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
class ENExposureConfiguration
```

## Mentioned in 

Supporting Exposure Notifications in iOS 12.5

## Overview

Important

This class is available in iOS 12.5, and in iOS 13.5 and later.

The ExposureNotification framework defines an Exposure Risk Value (ERV) to allow Health Authorities to define when to alert a user that they may have been exposed to someone diagnosed with COVID-19. The app uses the ERV to calculate the user’s Meaningful Exposure Minutes (MEMs) value. Health Authorities have flexibility in calculating this value by setting weights and values related to Bluetooth attenuations, infectiousness of the affected individual, and diagnosis report type. They can also determine what threshold will result in a notification.

Important

While the ERV is measured in MEMs, the system actually calculates and returns a number of seconds, rounded to the nearest minute. For example, if a person has an ERV of 2 MEMs, the app returns a value of 120 (seconds). Convert ERVs to minutes before displaying it to the user by dividing the returned value by 60.

The calculation method described in this document is available starting with iOS 14. To adopt this method of risk assessment, set the `ENAPIVersion` key to the integer value 2 in the app’s `Info.plist` file. For more information on the V1 calculation used in earlier versions of iOS, see Exposure Risk Value Calculation in ExposureNotification Version 1.

The following diagram shows how to calculate an ERV:

The class defines three sets of weights that give priority to the components of the ERV: minutes-at-attenuation, infectiousness, and report type.

The weighted minutes-at-attenuation assigns priority to the amount of time that the user is near beacons at different Bluetooth attenuations. Assign values between 0–250 percent to weights that represent Immediate, Near, Medium, and Other distances.

The infectiousness weight modifies the ERV based on the affected userʼs infectiousness level for the day of exposure relative to the day of symptom onset. To set the infectiousness level for when there is no symptom onset date provided, use ENDaysSinceOnsetOfSymptomsUnknown. A user’s infectiousness level can be ENInfectiousness.high, ENInfectiousness.standard, or ENInfectiousness.none. Assign both infectiousnessHighWeight and infectiousnessStandardWeight a value between 0 percent and 250 percent.

The weighted report type assigns priority to the method of diagnosis. Assign values ranging from 0–250 percent to weights that represent a confirmed test diagnosis, clinical diagnosis, self- reported diagnoisis, and recursive diagnosis.

In addition to setting the weights, you can perform additional filtering by setting daysSinceLastExposureThreshold to limit the number of days to consider when calculating the risk level.

### Calculating an Example Exposure Risk Value

The following diagrams illustrate calculating an ERV using a real-world scenario.

The weighted minutes-at-attenuation shows 5 minutes of immediate exposure with a 150 percent weight, 10 minutes of near exposure with a 100 percent weight, 10 minutes of medium exposure with a 50 percent weight, and 5 minutes of other exposure with a 0 percent weight.

The weighted infectiousness indicates days –14 to –6 from the current day with no infectiousness, days –5 to –3 with 100 percent of standard infectiousness, days –2 to +5 with 200 percent high infectiousness, days +6 to +10 with 100 percent standard infectiousness, and days +11 to +14 with no infectiousness.

Here are the weighted report types for all three tests:

The result of the calculation shows an ERV of 45 minutes:

Important

To prevent an ERV of 0, set any unused weight to 100 percent.

## Topics

### Configuring Duration

var attenuationDurationThresholds: [NSNumber]

The configurable signal-loss thresholds for calculating exposure risk.

var immediateDurationWeight: Double

The weight assigned to a risk level indicating the duration of the user’s exposure at immediate distance.

var mediumDurationWeight: Double

The weight assigned to a risk level indicating the duration of the user’s exposure at medium distance.

var nearDurationWeight: Double

The weight assigned to a risk level indicating the duration of the user’s exposure at close distance.

var otherDurationWeight: Double

The weight assigned to a risk level indicating the duration of the user’s exposure at a large distance.

var daysSinceLastExposureThreshold: Int

The number of days to consider when calculating the risk level.

### Configuring Infectiousness

var infectiousnessForDaysSinceOnsetOfSymptoms: [NSNumber : NSNumber]?

The mapping between the days since onset of symptoms to the degree of infectiousness.

var infectiousnessHighWeight: Double

The weight to apply for severe infectiousness.

var infectiousnessStandardWeight: Double

The weight to apply for mild infectiousness.

let ENDaysSinceOnsetOfSymptomsUnknown: Int

A value used when the number of days since onset of symptoms is unknown.

Deprecated

### Configuring Report Types

var reportTypeConfirmedClinicalDiagnosisWeight: Double

The weight assigned to a risk level based on a confirmed clinical diagnosis.

var reportTypeConfirmedTestWeight: Double

The weight assigned to a risk level based on a confirmed test.

var reportTypeRecursiveWeight: Double

The weight assigned to a risk level based on an exposure to someone exposed to someone else.

var reportTypeSelfReportedWeight: Double

The weight assigned to a risk level based on a self-reported diagnoisis.

var reportTypeNoneMap: ENDiagnosisReportType

The report type to map an unknown diagnosis to.

### Determining Exposure Risk Level in Version 1

Exposure Risk Value Calculation in ExposureNotification Version 1

Learn how to determine a user’s risk of exposure.

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

### Exposures

Configuring Exposure Notifications

Define how Exposure Notifications work for a region by assigning server-based key-value pairs.

class ENExposureWindow

A set of scan events from observed beacons within a time span.

class ENScanInstance

The aggregation of attenuations of beacons received during a scan.

Exposure Parameter Limits

The limits for the parameters you use in exposure risk calculations.


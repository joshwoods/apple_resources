

- HealthKit
-  HKMetadataKeyHeartRateRecoveryTestType 

Global Variable

# HKMetadataKeyHeartRateRecoveryTestType

The type of test that the source used to calculate a person’s heart-rate recovery.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
let HKMetadataKeyHeartRateRecoveryTestType: String
```

## Discussion

Use this metadata key to identify the type of test that the HKSource used to calculate the value for a heartRateRecoveryOneMinute sample.

## Topics

### Heart rate recovery tests

enum HKHeartRateRecoveryTestType

The test that measured a person’s heart-rate recovery.

## See Also

### Vitals Sensors Keys

let HKMetadataKeyBodyTemperatureSensorLocation: String

The location where a specific body temperature reading was taken.

let HKMetadataKeyHeartRateSensorLocation: String

The location where a specific heart rate reading was taken.

let HKMetadataKeyHeartRateMotionContext: String

The user’s activity level when the heart rate sample was measured.

let HKPredicateKeyPathAverageHeartRate: String

The key path for the sample’s average heart rate.

let HKMetadataKeyHeartRateRecoveryActivityDuration: String

let HKMetadataKeyHeartRateRecoveryActivityType: String

let HKMetadataKeyHeartRateRecoveryMaxObservedRecoveryHeartRate: String

let HKMetadataKeyVO2MaxTestType: String

The method used to calculate the user’s VO2 max rate.


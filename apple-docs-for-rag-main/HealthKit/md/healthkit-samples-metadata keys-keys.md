

- HealthKit
- Samples
-  Metadata Keys 

API Collection

# Metadata Keys

Constants used to add metadata to objects stored in HealthKit.

## Overview

Use these keys to facilitate sharing data between apps. You can also create your own custom keys to give HealthKit objects additional app-specific data.

## Topics

### General Keys

let HKMetadataKeyExternalUUID: String

A unique identifier for an HKObject that is set by its source.

let HKMetadataKeyTimeZone: String

The user’s time zone when the HealthKit object was created.

let HKMetadataKeyWasUserEntered: String

A key that indicates whether the sample was entered by the user.

let HKMetadataKeyQuantityClampedToLowerBound: String

let HKMetadataKeyQuantityClampedToUpperBound: String

### Estimate Keys

let HKMetadataKeyDateOfEarliestDataUsedForEstimate: String

The earliest date of data used to calculate the sample’s estimated value.

let HKMetadataKeySessionEstimate: String

### Device Information Keys

let HKMetadataKeyDeviceSerialNumber: String

The key for the serial number of the device that generated the data.

let HKMetadataKeyUDIDeviceIdentifier: String

The device identifier portion of a device’s UDI (unique device identifier).

let HKMetadataKeyUDIProductionIdentifier: String

The production identifier portion of a device’s UDI (unique device identifier).

let HKMetadataKeyDigitalSignature: String

A digital signature that can be used to validate the origin of the HealthKit object.

let HKMetadataKeyDeviceName: String

The name of the device that took this reading.

let HKMetadataKeyDeviceManufacturerName: String

The name of the manufacturer of the device that took this reading.

let HKMetadataKeyDevicePlacementSide: String

The key for metadata indicating the placement of the device that measured a sample.

enum HKDevicePlacementSide

Values that indicate the placement of the device that measured a sample.

let HKMetadataKeyAppleDeviceCalibrated: String

The key for metadata indicating whether the system had data from a sufficient amount of calibrated sensors when recording the sample.

### Sync Keys

let HKMetadataKeySyncIdentifier: String

A unique string that identifies a piece of data so it can be updated and synced.

let HKMetadataKeySyncVersion: String

The version number for a piece of data, used when updating or syncing.

### Lab Keys

let HKMetadataKeyWasTakenInLab: String

A key that indicates whether the sample was taken in a lab.

let HKMetadataKeyReferenceRangeLowerLimit: String

A key that indicates the lower limit of the reference range for a lab result.

let HKMetadataKeyReferenceRangeUpperLimit: String

A key that indicates the upper limit of the reference range for a lab result.

### Weather Keys

let HKMetadataKeyBarometricPressure: String

The metadata key for the barometric pressure associated with a sample.

let HKMetadataKeyWeatherCondition: String

A key that represents the weather condition during the sample.

let HKMetadataKeyWeatherHumidity: String

A key that represents the weather humidity during the sample.

let HKMetadataKeyWeatherTemperature: String

A key that represents the weather temperature during the sample.

### Workout Keys

Workout Metadata Keys

Constants that can be used to add metadata to workouts.

### Cardio Fitness Keys

let HKMetadataKeyVO2MaxValue: String

The maximum oxygen consumption rate during exercise of increasing intensity.

let HKMetadataKeyLowCardioFitnessEventThreshold: String

The VO2 max threshold used to categorize low-level cardio fitness events.

### Motion Keys

let HKMetadataKeyUserMotionContext: String

The person’s motion during the sample’s time period.

### Nutrition Keys

let HKMetadataKeyFoodType: String

The type of food that the HealthKit object represents.

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

let HKMetadataKeyHeartRateRecoveryTestType: String

The type of test that the source used to calculate a person’s heart-rate recovery.

let HKMetadataKeyVO2MaxTestType: String

The method used to calculate the user’s VO2 max rate.

### Audio Event Keys

let HKMetadataKeyAudioExposureLevel: String

The audio level associated with an audio event.

let HKMetadataKeyAudioExposureDuration: String

The audio exposure event’s duration.

let HKMetadataKeyHeadphoneGain: String

### Blood Glucose Keys

let HKMetadataKeyBloodGlucoseMealTime: String

A key that indicates the relative timing of a blood glucose reading to a meal.

let HKMetadataKeyInsulinDeliveryReason: String

The medical reason for administering insulin.

### Reproductive Health Keys

let HKMetadataKeyMenstrualCycleStart: String

A key that indicates whether the sample represents the start of a menstrual cycle. This metadata key is required for menstrualFlow category samples.

let HKMetadataKeySexualActivityProtectionUsed: String

A key that indicates whether protection was used during sexual activity. This metadata key can be used with sexualActivity category samples.

### Algorithm Keys

let HKMetadataKeyAlgorithmVersion: String

A key that indicates the version number of the algorithm used to calculate the sample’s value.

let HKMetadataKeyAppleECGAlgorithmVersion: String

A key for metadata indicating the version number of the algorithm Apple Watch uses to generate an ECG reading.

enum HKAppleECGAlgorithmVersion

Version numbers for the algorithm Apple Watch uses to generate an ECG reading.

let HKPredicateKeyPathECGClassification: String

The key path for the sample’s classification.

let HKPredicateKeyPathECGSymptomsStatus: String

The key path for the sample’s symptom status.

## See Also

### Basic samples

class HKCumulativeQuantitySample

A sample that represents a cumulative quantity.

class HKDiscreteQuantitySample

A sample that represents a discrete quantity.

class HKQuantitySample

A sample that represents a quantity, including the value and the units.

class HKCategorySample

A sample with values from a short list of possible values.

class HKCorrelation

A sample that groups multiple related samples into a single entry.

Units and quantities

Objects used to specify a quantity for a given unit, and to convert between units.


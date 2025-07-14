

- HealthKit
-  HKElectrocardiogram 

Class

# HKElectrocardiogram

A sample for electrocardiogram data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
class HKElectrocardiogram
```

## Overview

An HKElectrocardiogram is a collection of voltage values representing waveforms from one or more leads. The HKElectrocardiogram sample provides high-level details about the ECG reading, such as the sampling frequency or classification. HealthKit provides read-only access to electrocardiogram (ECG) data saved by Apple Watch.

You can query for HKElectrocardiogram samples using an HKSampleQuery.

```
// Create the electrocardiogram sample type.
let ecgType = HKObjectType.electrocardiogramType()

// Query for electrocardiogram samples
let ecgQuery = HKSampleQuery(sampleType: ecgType,
                             predicate: nil,
                             limit: HKObjectQueryNoLimit,
                             sortDescriptors: nil) { (query, samples, error) in
    if let error = error {
        // Handle the error here.
        fatalError("*** An error occurred \(error.localizedDescription) ***")
    }

    guard let ecgSamples = samples as? [HKElectrocardiogram] else {
        fatalError("*** Unable to convert \(String(describing: samples)) to [HKElectrocardiogram] ***")
    }

    for sample in ecgSamples {
        // Handle the samples here.

    }
}

// Execute the query.
healthStore.execute(ecgQuery)
```

After retrieving an HKElectrocardiogram sample, you can access the voltage measurements associated with the sample use an HKElectrocardiogramQuery query.

```
// Create a query for the voltage measurements
let voltageQuery = HKElectrocardiogramQuery(ecgSample) { (query, result) in
    switch(result) {

    case .measurement(let measurement):
        if let voltageQuantity = measurement.quantity(for: .appleWatchSimilarToLeadI) {
            // Do something with the voltage quantity here.

        }

    case .done:
        // No more voltage measurements. Finish processing the existing measurements.

    case .error(let error):
        // Handle the error here.

    }
}

// Execute the query.
healthStore.execute(voltageQuery)
```

## Topics

### Accessing Overview Information

var classification: HKElectrocardiogram.Classification

The ECG’s classification.

enum Classification

Classifications returned by Apple Watch’s ECG algorithm.

var averageHeartRate: HKQuantity?

The user’s average heart rate during the ECG.

var symptomsStatus: HKElectrocardiogram.SymptomsStatus

A value that indicates whether the user entered a symptom when they recorded the ECG.

enum SymptomsStatus

Values indicating whether the user entered a symptom when they recorded the ECG.

### Accessing Voltage Measurements

var numberOfVoltageMeasurements: Int

The number of voltage measurements associated with this sample.

var samplingFrequency: HKQuantity?

The frequency at which the Apple Watch sampled the voltage.

class VoltageMeasurement

The voltage for all leads at a single point in time.

enum Lead

The lead used to record a voltage measurement.

### Specifying Metadata

let HKMetadataKeyAppleECGAlgorithmVersion: String

A key for metadata indicating the version number of the algorithm Apple Watch uses to generate an ECG reading.

enum HKAppleECGAlgorithmVersion

Version numbers for the algorithm Apple Watch uses to generate an ECG reading.

### Specifying Predicate Key Paths

let HKPredicateKeyPathECGClassification: String

The key path for the sample’s classification.

let HKPredicateKeyPathECGSymptomsStatus: String

The key path for the sample’s symptom status.

let HKPredicateKeyPathAverageHeartRate: String

The key path for the sample’s average heart rate.

## Relationships

### Inherits From

- HKSample

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Electrocardiograms

class VoltageMeasurement

The voltage for all leads at a single point in time.


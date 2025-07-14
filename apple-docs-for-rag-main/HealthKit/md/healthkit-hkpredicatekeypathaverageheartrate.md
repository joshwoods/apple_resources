

- HealthKit
-  HKPredicateKeyPathAverageHeartRate 

Global Variable

# HKPredicateKeyPathAverageHeartRate

The key path for the sample’s average heart rate.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
let HKPredicateKeyPathAverageHeartRate: String
```

## Discussion

Use this constant whenever you want to include the ECG’s average heart rate in a predicate format string. Add a `%K` placeholder to the format string, and then pass this constant as an argument.

## See Also

### Specifying Predicate Key Paths

let HKPredicateKeyPathECGClassification: String

The key path for the sample’s classification.

let HKPredicateKeyPathECGSymptomsStatus: String

The key path for the sample’s symptom status.


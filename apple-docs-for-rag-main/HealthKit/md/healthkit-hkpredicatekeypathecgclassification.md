

- HealthKit
-  HKPredicateKeyPathECGClassification 

Global Variable

# HKPredicateKeyPathECGClassification

The key path for the sample’s classification.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
let HKPredicateKeyPathECGClassification: String
```

## Discussion

Use this constant whenever you want to include the ECG’s classification in a predicate format string. Add a `%K` placeholder to the format string, and then pass this constant as an argument.

## See Also

### Related Documentation

enum Classification

Classifications returned by Apple Watch’s ECG algorithm.

### Specifying Predicate Key Paths

let HKPredicateKeyPathECGSymptomsStatus: String

The key path for the sample’s symptom status.

let HKPredicateKeyPathAverageHeartRate: String

The key path for the sample’s average heart rate.




- HealthKit
- HKCorrelationTypeIdentifier
-  food 

Type Property

# food

Food correlation types combine any number of nutritional samples into a single food object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
static let food: HKCorrelationTypeIdentifier
```

## Discussion

When creating food samples, specify the type of food using the HKMetadataKeyFoodType metadata key.

## See Also

### Related Documentation

struct HKCorrelationTypeIdentifier

The identifiers that create correlation type objects.

class HKCorrelationType

A type that identifies samples that group multiple subsamples.

class HKCorrelation

A sample that groups multiple related samples into a single entry.

### Essentials

let HKMetadataKeyFoodType: String

The type of food that the HealthKit object represents.


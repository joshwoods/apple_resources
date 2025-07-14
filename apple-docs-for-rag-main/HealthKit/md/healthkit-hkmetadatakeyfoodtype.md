

- HealthKit
-  HKMetadataKeyFoodType 

Global Variable

# HKMetadataKeyFoodType

The type of food that the HealthKit object represents.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
let HKMetadataKeyFoodType: String
```

## Discussion

This key takes a string value. Food objects are usually food samples containing any number of `Nutrition Identifiers` samples.

## See Also

### Essentials

static let food: HKCorrelationTypeIdentifier

Food correlation types combine any number of nutritional samples into a single food object.


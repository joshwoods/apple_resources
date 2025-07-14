

- HealthKit
- HKCorrelation
-  objects 

Instance Property

# objects

The set of sample objects that make up the correlation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var objects: Set { get }
```

## Discussion

This property contains the quantity and category samples that are grouped into this correlation. Blood pressure correlations always include two quantity samples that represent the systolic and diastolic values. In contrast, food correlations can contain a wide range of dietary information about the food, including information about the fat, protein, carbohydrates, energy, and vitamins consumed.

## See Also

### Getting Correlation Data

var correlationType: HKCorrelationType

The type for this correlation.

func objects(for: HKObjectType) -> Set&lt;HKSample>

Returns a set containing all the objects of the specified type in the correlation.


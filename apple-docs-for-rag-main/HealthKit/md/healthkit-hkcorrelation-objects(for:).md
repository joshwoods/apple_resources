

- HealthKit
- HKCorrelation
-  objects(for:) 

Instance Method

# objects(for:)

Returns a set containing all the objects of the specified type in the correlation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
func objects(for objectType: HKObjectType) -> Set
```

## Parameters 

`objectType`  

The quantity or category type for the data stored inside the correlation. For example, to get all the samples measuring calories from inside a correlation, use an HKSampleType object created with the dietaryEnergyConsumed identifier.

## Return Value

A set containing all the objects of the specified type in the correlation.

## See Also

### Getting Correlation Data

var correlationType: HKCorrelationType

The type for this correlation.

var objects: Set&lt;HKSample>

The set of sample objects that make up the correlation.


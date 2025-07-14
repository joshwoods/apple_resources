

- HealthKit
- HKCorrelation
-  correlationType 

Instance Property

# correlationType

The type for this correlation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var correlationType: HKCorrelationType { get }
```

## Discussion

For a complete list of correlation types, see Correlation Identifiers in HealthKit Constants.

## See Also

### Getting Correlation Data

var objects: Set&lt;HKSample>

The set of sample objects that make up the correlation.

func objects(for: HKObjectType) -> Set&lt;HKSample>

Returns a set containing all the objects of the specified type in the correlation.


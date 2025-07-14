

- HealthKit
- HKCorrelationQuery
-  samplePredicates 

Instance Property

# samplePredicates

A dictionary whose keys are HKSampleType instances and whose values are NSPredicate instances.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var samplePredicates: [HKSampleType : NSPredicate]? { get }
```

## Discussion

The query uses this dictionary to perform complex tests against the correlation’s contents. For more information, see init(type:predicate:samplePredicates:completion:).

## See Also

### Getting Property Data

var correlationType: HKCorrelationType

The type of correlation to search for.


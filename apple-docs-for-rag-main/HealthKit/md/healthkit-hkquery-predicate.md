

- HealthKit
- HKQuery
-  predicate 

Instance Property

# predicate

A predicate used to filter the objects returned from the HealthKit store.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var predicate: NSPredicate? { get }
```

## Discussion

If the predicate is `nil`, the query does not filter its results. Instead, it returns all the objects matching the query’s other parameters.

## See Also

### Accessing properties

var objectType: HKObjectType?

The type of objects being queried.

var sampleType: HKSampleType?

The type of objects being queried.

Deprecated


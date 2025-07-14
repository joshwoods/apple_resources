

- HealthKit
- HKSampleQueryDescriptor
-  limit 

Instance Property

# limit

The maximum number of samples that the query returns.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
var limit: Int?
```

## Discussion

If the `limit` is `nil`, the system returns all matching samples in the HealthKit store.

## See Also

### Accessing Query Properties

var predicates: [HKSamplePredicate&lt;Sample>]

An array of sample predicates that define the type of data that the query returns.

var sortDescriptors: [SortDescriptor&lt;Sample>]

An array that specifies the order of the results that the query returns.


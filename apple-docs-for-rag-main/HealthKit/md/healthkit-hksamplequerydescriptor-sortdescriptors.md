

- HealthKit
- HKSampleQueryDescriptor
-  sortDescriptors 

Instance Property

# sortDescriptors

An array that specifies the order of the results that the query returns.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
var sortDescriptors: [SortDescriptor]
```

## Discussion

The system applies the sort descriptors in order. The later descriptors sort any items that the earlier sort descriptors considered equal. If you don’t need the results in a specific order, pass an empty array.

## See Also

### Accessing Query Properties

var limit: Int?

The maximum number of samples that the query returns.

var predicates: [HKSamplePredicate&lt;Sample>]

An array of sample predicates that define the type of data that the query returns.


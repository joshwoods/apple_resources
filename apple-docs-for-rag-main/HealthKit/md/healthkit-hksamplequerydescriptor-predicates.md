

- HealthKit
- HKSampleQueryDescriptor
-  predicates 

Instance Property

# predicates

An array of sample predicates that define the type of data that the query returns.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
var predicates: [HKSamplePredicate] { get set }
```

## Discussion

To query for multiple types of data, provide a sample predicate for each type. If your HKSamplePredicate instances return different HKSample subclasses, use sample(type:predicate:) to create the sample predicates.

## See Also

### Accessing Query Properties

var limit: Int?

The maximum number of samples that the query returns.

var sortDescriptors: [SortDescriptor&lt;Sample>]

An array that specifies the order of the results that the query returns.


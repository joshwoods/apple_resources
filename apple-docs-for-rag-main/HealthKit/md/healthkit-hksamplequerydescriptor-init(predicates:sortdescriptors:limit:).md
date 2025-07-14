

- HealthKit
- HKSampleQueryDescriptor
-  init(predicates:sortDescriptors:limit:) 

Initializer

# init(predicates:sortDescriptors:limit:)

Creates a sample query descriptor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
init(
    predicates: [HKSamplePredicate],
    sortDescriptors: [SortDescriptor],
    limit: Int? = nil
)
```

## Parameters 

`predicates`  

An array of sample predicates that define the type of data that the query returns. To query for multiple types of data, provide a sample predicate for each type.

`sortDescriptors`  

An array of sort descriptors that specify the order of the results that the query returns. If you don’t need the results in a specific order, pass an empty array.

`limit`  

An optional value that specifies the maximum number of samples that the query returns. If you don’t specify the limit, the system returns all matching samples in the HealthKit store.

## Discussion

The system sets the descriptor’s `HKSampleQueryDescriptor/Output` type based on the `predicates` parameter.


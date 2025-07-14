

- HealthKit
- HKAnchoredObjectQueryDescriptor
-  init(predicates:anchor:limit:) 

Initializer

# init(predicates:anchor:limit:)

Creates an anchored object query descriptor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
init(
    predicates: [HKSamplePredicate],
    anchor: HKQueryAnchor?,
    limit: Int? = nil
)
```

## Parameters 

`predicates`  

An array of sample predicates that define the type of data that the query returns. To query for multiple types of data, provide a sample predicate for each type.

`anchor`  

An anchor that a previous anchored object query returned. The anchor object corresponds to the last object that the previous query returned. The current query returns only samples and deleted objects newer than the anchor. Pass `nil` to receive all the matching samples and recently deleted objects currently in the HealthKit store.

`limit`  

An optional value that specifies the maximum number of samples that the query returns. If you don’t specify the limit, the system returns all matching samples in the HealthKit store.

## Discussion

The system sets the descriptor’s `HKAnchoredObjectQueryDescriptor/Output` type based on the `predicates` parameter.




- HealthKit
- HKAnchoredObjectQueryDescriptor
-  anchor 

Instance Property

# anchor

An anchor that a previous anchored object query returned.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
var anchor: HKQueryAnchor?
```

## Discussion

The anchor object corresponds to the last object that the previous query returned. The current query returns only samples and deleted objects newer than the anchor. Pass `nil` to receive all the matching samples and recently deleted objects currently in the HealthKit store.

## See Also

### Accessing Query Properties

var predicates: [HKSamplePredicate&lt;Sample>]

A predicate that limits the results that the query returns.

var limit: Int?

The maximum number of samples that the query returns.




- HealthKit
- HKWorkoutEffortRelationshipQuery
-  init(predicate:anchor:options:resultsHandler:) 

Initializer

# init(predicate:anchor:options:resultsHandler:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    predicate: NSPredicate?,
    anchor: HKQueryAnchor?,
    options: HKWorkoutEffortRelationshipQueryOptions,
    resultsHandler: @escaping (HKWorkoutEffortRelationshipQuery, [HKWorkoutEffortRelationship]?, HKQueryAnchor?, (any Error)?) -> Void
)
```


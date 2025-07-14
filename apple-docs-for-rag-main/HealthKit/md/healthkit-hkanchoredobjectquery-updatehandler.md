

- HealthKit
- HKAnchoredObjectQuery
-  updateHandler 

Instance Property

# updateHandler

Handler for monitoring updates to the HealthKit store.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOSvisionOS 1.0+watchOS 2.0+

``` source
var updateHandler: ((HKAnchoredObjectQuery, [HKSample]?, [HKDeletedObject]?, HKQueryAnchor?, (any Error)?) -> Void)? { get set }
```

## Discussion

If this property is set to `nil`, the anchor query automatically stops as soon as it finishes calculating the initial results. If this property is not `nil`, the query behaves similarly to the observer query: it continues to run, monitoring the HealthKit store. The system executes the update handler on a background queue whenever matching samples are saved to or deleted from the HealthKit store.


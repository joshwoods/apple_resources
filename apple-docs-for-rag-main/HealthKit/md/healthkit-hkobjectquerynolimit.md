

- HealthKit
-  HKObjectQueryNoLimit 

Global Variable

# HKObjectQueryNoLimit

A value indicating that the query returns all the matching samples in the HealthKit store.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
let HKObjectQueryNoLimit: Int
```

## See Also

### Creating Anchored Object Queries

Executing Anchored Object Queries

Create and run an anchored object query.

init(type: HKSampleType, predicate: NSPredicate?, anchor: HKQueryAnchor?, limit: Int, resultsHandler: (HKAnchoredObjectQuery, [HKSample]?, [HKDeletedObject]?, HKQueryAnchor?, (any Error)?) -> Void)

Initializes a new anchored object query.

init(queryDescriptors: [HKQueryDescriptor], anchor: HKQueryAnchor?, limit: Int, resultsHandler: (HKAnchoredObjectQuery, [HKSample]?, [HKDeletedObject]?, HKQueryAnchor?, (any Error)?) -> Void)

Creates an anchored object query that matches any of the query descriptors you provided.

init(type: HKSampleType, predicate: NSPredicate?, anchor: Int, limit: Int, completionHandler: (HKAnchoredObjectQuery, [HKSample]?, Int, (any Error)?) -> Void)

Initializes a new anchored object query.

Deprecated


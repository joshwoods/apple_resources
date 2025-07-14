

- HealthKit
-  HKAnchoredObjectQuery 

Class

# HKAnchoredObjectQuery

A query that returns changes to the HealthKit store, including a snapshot of new changes and continuous monitoring as a long-running query.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class HKAnchoredObjectQuery
```

## Mentioned in 

About the HealthKit framework

Receiving Downhill Skiing and Snowboarding Data

Executing Observer Queries

## Overview

Anchored object queries provide an easy way to search for new data in the HealthKit store. An HKAnchoredObjectQuery returns an anchor value that corresponds to the last sample or deleted object received by that query. Subsequent queries can use this anchor to restrict their results to only newer saved or deleted objects.

Anchored object queries are mostly immutable. You can assign the query’s updateHandler property after instantiating the object, but you must set all other properties when you instantiate the object. You can’t change them.

### Combine Snapshots and Updates

The anchored object query can combine the abilities of a regular query with a long-running query.

- It grabs a snapshot of the data currently stored in the HealthKit store (like an HKSampleQuery).

- It can also perform a long-running query that responds to updates (like an HKObserverQuery).

Often, it’s more efficient to set up and run a single anchored object query than to run separate sample and observer queries. As a result, you may want to use anchored object queries, even when you aren’t using anchors to limit the results. In this case, set the anchor parameter to `nil`.

## Topics

### Creating Anchored Object Queries

Executing Anchored Object Queries

Create and run an anchored object query.

init(type: HKSampleType, predicate: NSPredicate?, anchor: HKQueryAnchor?, limit: Int, resultsHandler: (HKAnchoredObjectQuery, [HKSample]?, [HKDeletedObject]?, HKQueryAnchor?, (any Error)?) -> Void)

Initializes a new anchored object query.

init(queryDescriptors: [HKQueryDescriptor], anchor: HKQueryAnchor?, limit: Int, resultsHandler: (HKAnchoredObjectQuery, [HKSample]?, [HKDeletedObject]?, HKQueryAnchor?, (any Error)?) -> Void)

Creates an anchored object query that matches any of the query descriptors you provided.

let HKObjectQueryNoLimit: Int

A value indicating that the query returns all the matching samples in the HealthKit store.

init(type: HKSampleType, predicate: NSPredicate?, anchor: Int, limit: Int, completionHandler: (HKAnchoredObjectQuery, [HKSample]?, Int, (any Error)?) -> Void)

Initializes a new anchored object query.

Deprecated

### Receiving Updates

var updateHandler: ((HKAnchoredObjectQuery, [HKSample]?, [HKDeletedObject]?, HKQueryAnchor?, (any Error)?) -> Void)?

Handler for monitoring updates to the HealthKit store.

### Tracking Anchors

class HKQueryAnchor

An object used to identify all the samples previously returned by an anchored object query.

### Tracking Deleted Objects

class HKDeletedObject

An object that represents a sample that has been deleted from the HealthKit store.

## Relationships

### Inherits From

- HKQuery

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Long-running queries

struct HKActivitySummaryQueryDescriptor

A query interface that reads activity summaries using Swift concurrency.

class HKActivitySummaryQuery

A query for reading activity summary objects from the HealthKit store.

struct HKAnchoredObjectQueryDescriptor

A query interface that runs anchored object queries using Swift concurrency.

class HKObserverQuery

A long-running query that monitors the HealthKit store and updates your app when the HealthKit store saves or deletes a matching sample.


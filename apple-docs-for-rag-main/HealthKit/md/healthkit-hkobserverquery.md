

- HealthKit
-  HKObserverQuery 

Class

# HKObserverQuery

A long-running query that monitors the HealthKit store and updates your app when the HealthKit store saves or deletes a matching sample.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKObserverQuery
```

## Mentioned in 

Reading data from HealthKit

## Overview

Observer queries set up a long-running task on a background queue. This task watches the HealthKit store, and alerts you when the store saves or removes matching data. Your app uses observer queries to respond to changes made by other apps and devices.

Important

Background server queries aren’t supported on the Simulator. Be sure to test your background queries on a device.

Observer queries are immutable: You set their properties when you first create them, and you can’t change them.

## Topics

### Creating Observer Queries

Executing Observer Queries

Create and run observer queries.

init(sampleType: HKSampleType, predicate: NSPredicate?, updateHandler: (HKObserverQuery, HKObserverQueryCompletionHandler, (any Error)?) -> Void)

Instantiates and returns a query that monitors the HealthKit store and responds to changes.

init(queryDescriptors: [HKQueryDescriptor], updateHandler: (HKObserverQuery, Set&lt;HKSampleType>?, HKObserverQueryCompletionHandler, (any Error)?) -> Void)

Creates a query that monitors the HealthKit store and responds to any changes matching any of the query descriptors you provided.

typealias HKObserverQueryCompletionHandler

The completion handler for background deliveries.

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

class HKAnchoredObjectQuery

A query that returns changes to the HealthKit store, including a snapshot of new changes and continuous monitoring as a long-running query.


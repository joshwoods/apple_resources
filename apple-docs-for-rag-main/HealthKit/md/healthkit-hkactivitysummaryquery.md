

- HealthKit
-  HKActivitySummaryQuery 

Class

# HKActivitySummaryQuery

A query for reading activity summary objects from the HealthKit store.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class HKActivitySummaryQuery
```

## Overview

Activity summary query objects are mostly immutable. You can assign the query’s updateHandler property after instantiating the object, but before executing the query. All other properties must be set when you instantiate the object, and they can’t change.

## Topics

### Creating activity summary queries

Executing Activity Summary Queries

Create and run activity summary queries.

init(predicate: NSPredicate?, resultsHandler: (HKActivitySummaryQuery, [HKActivitySummary]?, (any Error)?) -> Void)

Initializes a new active summary query.

### Getting property data

var updateHandler: ((HKActivitySummaryQuery, [HKActivitySummary]?, (any Error)?) -> Void)?

The handler for monitoring updates to activity summaries saved in the HealthKit store.

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

struct HKAnchoredObjectQueryDescriptor

A query interface that runs anchored object queries using Swift concurrency.

class HKAnchoredObjectQuery

A query that returns changes to the HealthKit store, including a snapshot of new changes and continuous monitoring as a long-running query.

class HKObserverQuery

A long-running query that monitors the HealthKit store and updates your app when the HealthKit store saves or deletes a matching sample.


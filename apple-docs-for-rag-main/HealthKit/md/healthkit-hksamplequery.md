

- HealthKit
-  HKSampleQuery 

Class

# HKSampleQuery

A general query that returns a snapshot of all the matching samples currently saved in the HealthKit store.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class HKSampleQuery
```

## Mentioned in 

Executing Observer Queries

## Overview

You can use sample queries to search for any concrete subclasses of the HKSample class, including HKCategorySample, HKCorrelation, HKQuantitySample, and HKWorkout objects.

The sample query returns sample objects that match the provided type and predicate. You can provide a sort order for the returned samples, or limit the number of samples returned. Other query classes can be used to perform more specialized searches and calculations. For more information, see HKQuery.

Sample queries are immutable: The query’s properties are set when the query is first created, and they can’t change.

Note

Like many HealthKit classes, the HKSampleQuery class should not be subclassed.

## Topics

### Creating Sample Queries

Executing Sample Queries

Create, run, and sort sample queries.

init(sampleType: HKSampleType, predicate: NSPredicate?, limit: Int, sortDescriptors: [NSSortDescriptor]?, resultsHandler: (HKSampleQuery, [HKSample]?, (any Error)?) -> Void)

Instantiates and returns a sample query.

init(queryDescriptors: [HKQueryDescriptor], limit: Int, resultsHandler: (HKSampleQuery, [HKSample]?, (any Error)?) -> Void)

Creates a query for samples that match any of the descriptors you provided.

init(queryDescriptors: [HKQueryDescriptor], limit: Int, sortDescriptors: [NSSortDescriptor], resultsHandler: (HKSampleQuery, [HKSample]?, (any Error)?) -> Void)

Creates a query for samples that match any of the query descriptors you provided, sorted by the sort descriptors you provided.

let HKObjectQueryNoLimit: Int

A value indicating that the query returns all the matching samples in the HealthKit store.

HealthKit sort descriptors

Identifiers for sorting results.

### Getting Property Data

var limit: Int

The maximum number of samples that this query returns.

var sortDescriptors: [NSSortDescriptor]?

The sort descriptors that specify the order of the results returned by this query.

### Setting Limits

let HKObjectQueryNoLimit: Int

A value indicating that the query returns all the matching samples in the HealthKit store.

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

### Basic queries

struct HKSampleQueryDescriptor

A query interface that reads samples using Swift concurrency.

class HKCorrelationQuery

A query that performs complex searches based on the correlation’s contents, and returns a snapshot of all matching samples.

class HKQueryDescriptor

A descriptor that specifies a set of samples based on the data type and a predicate.

class HKQuery

An abstract class for all the query classes in HealthKit.


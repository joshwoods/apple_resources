

- HealthKit
-  HKQuantitySeriesSampleQuery 

Class

# HKQuantitySeriesSampleQuery

A query that accesses the series data associated with a quantity sample.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class HKQuantitySeriesSampleQuery
```

## Mentioned in 

Accessing condensed workout samples

## Overview

Use a series query to access the individual HKQuantity objects added to a sample using an HKQuantitySeriesSampleBuilder.

Important

For many common calculations, consider using a statistical query instead. Statistical queries correctly handle quantity data, whether the samples represent a single quantity or a series.

## Topics

### Creating a Series Query

init(quantityType: HKQuantityType, predicate: NSPredicate?, quantityHandler: (HKQuantitySeriesSampleQuery, HKQuantity?, DateInterval?, HKQuantitySample?, Bool, (any Error)?) -> Void)

Creates a new query for a series of the specified quantity type.

var includeSample: Bool

A Boolean value that determines whether the query should return the series sample.

var orderByQuantitySampleStartDate: Bool

A Boolean value that determines whether the query groups the results based on the quantity sample’s start date.

### Deprecated Mehtods

init(sample: HKQuantitySample, quantityHandler: (HKQuantitySeriesSampleQuery, HKQuantity?, Date?, Bool, (any Error)?) -> Void)

Creates a new series query.

Deprecated

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

### Related Documentation

class HKQuantitySeriesSampleBuilder

A builder object for incrementally building a sample that contains multiple quantities.

class HKCumulativeQuantitySample

A sample that represents a cumulative quantity.

class HKDiscreteQuantitySample

A sample that represents a discrete quantity.

### Series queries

struct HKQuantitySeriesSampleQueryDescriptor

A query interface that reads the series data associated with quantity samples using Swift concurrency.

struct HKWorkoutRouteQueryDescriptor

A query interface that reads the location data stored in a workout route using Swift concurrency.

class HKWorkoutRouteQuery

A query to access the location data stored in a workout route.

struct HKHeartbeatSeriesQueryDescriptor

A query interface that reads the heartbeat series data stored in a heartbeat sample using Swift concurrency.

class HKHeartbeatSeriesQuery

A query that returns the heartbeat data contained in a heartbeat series sample.

struct HKElectrocardiogramQueryDescriptor

A query interface that reads the underlying voltage measurements for an electrocardiogram sample using Swift concurrency.

class HKElectrocardiogramQuery

A query that returns the underlying voltage measurements for an electrocardiogram sample.


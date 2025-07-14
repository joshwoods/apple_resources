

- HealthKit
-  HKWorkoutRouteQuery 

Class

# HKWorkoutRouteQuery

A query to access the location data stored in a workout route.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class HKWorkoutRouteQuery
```

## Mentioned in 

Reading route data

## Overview

Use a workout route query to access the location data associated with an HKWorkoutRoute. Because a route sample can include a large number of CLLocation objects, the query asynchronously returns the locations in batches. For detailed instructions, see `Reading Route Data`.

## Topics

### Creating route queries

init(route: HKWorkoutRoute, dataHandler: (HKWorkoutRouteQuery, [CLLocation]?, Bool, (any Error)?) -> Void)

Creates a new query to access the location data associated with a workout route.

init(route: HKWorkoutRoute, dateInterval: DateInterval, dataHandler: (HKWorkoutRouteQuery, [CLLocation]?, Bool, (any Error)?) -> Void)

Creates a new query to access the location data associated with a workout route during the specified date interval.

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

### Series queries

struct HKQuantitySeriesSampleQueryDescriptor

A query interface that reads the series data associated with quantity samples using Swift concurrency.

class HKQuantitySeriesSampleQuery

A query that accesses the series data associated with a quantity sample.

struct HKWorkoutRouteQueryDescriptor

A query interface that reads the location data stored in a workout route using Swift concurrency.

struct HKHeartbeatSeriesQueryDescriptor

A query interface that reads the heartbeat series data stored in a heartbeat sample using Swift concurrency.

class HKHeartbeatSeriesQuery

A query that returns the heartbeat data contained in a heartbeat series sample.

struct HKElectrocardiogramQueryDescriptor

A query interface that reads the underlying voltage measurements for an electrocardiogram sample using Swift concurrency.

class HKElectrocardiogramQuery

A query that returns the underlying voltage measurements for an electrocardiogram sample.


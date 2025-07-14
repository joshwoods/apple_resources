

- HealthKit
-  HKHeartbeatSeriesQuery 

Class

# HKHeartbeatSeriesQuery

A query that returns the heartbeat data contained in a heartbeat series sample.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class HKHeartbeatSeriesQuery
```

## Topics

### Creating a Heartbeat Series Query

init(heartbeatSeries: HKHeartbeatSeriesSample, dataHandler: (HKHeartbeatSeriesQuery, TimeInterval, Bool, Bool, (any Error)?) -> Void)

Creates a new heartbeat series query.

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

class HKWorkoutRouteQuery

A query to access the location data stored in a workout route.

struct HKHeartbeatSeriesQueryDescriptor

A query interface that reads the heartbeat series data stored in a heartbeat sample using Swift concurrency.

struct HKElectrocardiogramQueryDescriptor

A query interface that reads the underlying voltage measurements for an electrocardiogram sample using Swift concurrency.

class HKElectrocardiogramQuery

A query that returns the underlying voltage measurements for an electrocardiogram sample.




- HealthKit
-  HKElectrocardiogramQuery 

Class

# HKElectrocardiogramQuery

A query that returns the underlying voltage measurements for an electrocardiogram sample.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class HKElectrocardiogramQuery
```

## Overview

Use the HKElectrocardiogramQuery query to access the individual voltage measurements associated with an HKElectrocardiogram sample.

```
// Create a query for the voltage measurements
let voltageQuery = HKElectrocardiogramQuery(ecgSample) { (query, result) in
    switch(result) {

    case .measurement(let measurement):
        if let voltageQuantity = measurement.quantity(for: .appleWatchSimilarToLeadI) {
            // Do something with the voltage quantity here.

        }

    case .done:
        // No more voltages. Finish processing the existing voltages.

    case .error(let error):
        // Handle the error here.

    }
}

// Execute the query.
healthStore.execute(voltageQuery)
```

The query calls the data handler once for each voltage measurement, passing a HKElectrocardiogramQuery.Result.measurement(_:) instance that contains the voltage data. After it has sent all the voltage measurements, the query calls the data handler one last time, passing HKElectrocardiogramQuery.Result.done. If an error occurs, it stops collecting voltage data and passes HKElectrocardiogramQuery.Result.error(_:) instead.

Electrocardiogram queries are immutable: You set query’s properties when you create it, and they don’t change.

## Topics

### Creating the Query

convenience init(HKElectrocardiogram, dataHandler: (HKElectrocardiogramQuery, HKElectrocardiogramQuery.Result) -> Void)

Creates a new electrocardiogram query object.

### Accessing the Results

enum Result

Partial results for an electrocardiogram query.

init(electrocardiogram: HKElectrocardiogram, dataHandler: (HKElectrocardiogramQuery, HKElectrocardiogram.VoltageMeasurement?, Bool, (any Error)?) -> Void)

Creates a new electrocardiogram query object.

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

class HKHeartbeatSeriesQuery

A query that returns the heartbeat data contained in a heartbeat series sample.

struct HKElectrocardiogramQueryDescriptor

A query interface that reads the underlying voltage measurements for an electrocardiogram sample using Swift concurrency.


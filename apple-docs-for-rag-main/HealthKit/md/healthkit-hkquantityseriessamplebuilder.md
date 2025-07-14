

- HealthKit
-  HKQuantitySeriesSampleBuilder 

Class

# HKQuantitySeriesSampleBuilder

A builder object for incrementally building a sample that contains multiple quantities.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 5.0+

``` source
class HKQuantitySeriesSampleBuilder
```

## Topics

### Creating a Quantity Series Builder

init(healthStore: HKHealthStore, quantityType: HKQuantityType, startDate: Date, device: HKDevice?)

Creates a new quantity series builder.

var quantityType: HKQuantityType

The quantity type for the series.

var startDate: Date

The starting date and time for the sample.

var device: HKDevice?

The device providing the data.

### Adding Values

func insert(HKQuantity, at: Date) throws

Adds a new quantity to the series at the provided date and time.

func insert(HKQuantity, for: DateInterval) throws

Adds a new quantity to the series with the provided date interval.

### Ending the Collection

func discard()

Discards all previously collected data and invalidates the builder.

func finishSeries(metadata: [String : Any]?, completion: ([HKQuantitySample]?, (any Error)?) -> Void)

Finalizes the series and returns the resulting quantity samples.

func finishSeries(metadata: [String : Any]?, endDate: Date?, completion: ([HKQuantitySample]?, (any Error)?) -> Void)

Finalizes the series with the provided end date, and returns the resulting quantity samples.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Series data

class HKHeartbeatSeriesBuilder

A builder object for incrementally building a heartbeat series.

class HKHeartbeatSeriesSample

A sample that represents a series of heartbeats.


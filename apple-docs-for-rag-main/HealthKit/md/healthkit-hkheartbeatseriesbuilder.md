

- HealthKit
-  HKHeartbeatSeriesBuilder 

Class

# HKHeartbeatSeriesBuilder

A builder object for incrementally building a heartbeat series.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class HKHeartbeatSeriesBuilder
```

## Topics

### Creating a Heartbeat Series Builder

init(healthStore: HKHealthStore, device: HKDevice?, start: Date)

Creates a new heartbeat series builder.

class var maximumCount: Int

The maximum number of heartbeats you can add to the sample.

### Adding Data

func addHeartbeatWithTimeInterval(sinceSeriesStartDate: TimeInterval, precededByGap: Bool, completion: (Bool, (any Error)?) -> Void)

Adds a heartbeat to the series.

func addMetadata([String : Any], completion: (Bool, (any Error)?) -> Void)

Adds metadata to the sample.

### Ending the Collection

func finishSeries(completion: (HKHeartbeatSeriesSample?, (any Error)?) -> Void)

Finalizes the series and returns the resulting heartbeat series sample.

## Relationships

### Inherits From

- HKSeriesBuilder

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

class HKQuantitySeriesSampleBuilder

A builder object for incrementally building a sample that contains multiple quantities.

class HKHeartbeatSeriesSample

A sample that represents a series of heartbeats.


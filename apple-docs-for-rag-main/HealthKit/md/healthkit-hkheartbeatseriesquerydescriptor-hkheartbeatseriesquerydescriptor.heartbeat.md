

- HealthKit
- HKHeartbeatSeriesQueryDescriptor
-  HKHeartbeatSeriesQueryDescriptor.Heartbeat 

Structure

# HKHeartbeatSeriesQueryDescriptor.Heartbeat

Data about an individual heartbeat.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct Heartbeat
```

## Topics

### Accessing Heartbeat Data

let precededByGap: Bool

let timeIntervalSinceStart: TimeInterval

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Running Queries

func results(for: HKHealthStore) -> HKHeartbeatSeriesQueryDescriptor.Results

Runs a one-shot query that returns an asynchronous sequence of data representing individual heartbeats.

struct Results

An asynchronous sequence that emits data about individual heartbeats from a heartbeat series sample.


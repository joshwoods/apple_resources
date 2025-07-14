

- HealthKit
- HKHeartbeatSeriesQueryDescriptor
-  HKHeartbeatSeriesQueryDescriptor.Results 

Structure

# HKHeartbeatSeriesQueryDescriptor.Results

An asynchronous sequence that emits data about individual heartbeats from a heartbeat series sample.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct Results
```

## Topics

### Creating an Iterator

struct Iterator

An iterator for accessing individual data entries from the series.

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Running Queries

func results(for: HKHealthStore) -> HKHeartbeatSeriesQueryDescriptor.Results

Runs a one-shot query that returns an asynchronous sequence of data representing individual heartbeats.

struct Heartbeat

Data about an individual heartbeat.


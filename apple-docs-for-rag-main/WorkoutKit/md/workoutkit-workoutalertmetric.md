

- WorkoutKit
-  WorkoutAlertMetric 

Enumeration

# WorkoutAlertMetric

A value that specifies the type of metric used to measure performance.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
enum WorkoutAlertMetric
```

## Topics

### Determining the metric’s type

case average

The metric represents an average value.

case current

The metric represents the current value.

### Accessing the metric’s value

static var countPerMinute: UnitFrequency

The metric’s counts per minute.

### Comparing metrics

static func == (WorkoutAlertMetric, WorkoutAlertMetric) -> Bool

Returns a Boolean value that indicates whether two workout metrics are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two workout metrics aren’t equal.

var hashValue: Int

The hashed value of the workout metric.

func hash(into: inout Hasher)

Hashes the essential components of the workout metric by feeding them into the given hash function.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Setting the alert metric

var metric: WorkoutAlertMetric

The metric used to measure performance for the alert.

**Required**


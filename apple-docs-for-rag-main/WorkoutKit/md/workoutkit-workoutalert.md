

- WorkoutKit
-  WorkoutAlert 

Protocol

# WorkoutAlert

An alert that notifies the user of significant events during a workout.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
protocol WorkoutAlert : Hashable, Sendable
```

## Topics

### Determining support

func supports(activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType) -> Bool

Returns a Boolean value that indicates whether the alert supports the provided activity and location.

**Required**

### Setting the alert metric

var metric: WorkoutAlertMetric

The metric used to measure performance for the alert.

**Required**

enum WorkoutAlertMetric

A value that specifies the type of metric used to measure performance.

### Creating cadence alerts

static func cadence(ClosedRange&lt;Double>, unit: UnitFrequency) -> Self

Creates a new alert for a range of cadence values.

struct CadenceRangeAlert

An alert for a range of cadence values.

static func cadence(Double, unit: UnitFrequency) -> Self

Creates an alert for the specified cadence threshold.

struct CadenceThresholdAlert

An alert for a cadence threshold.

### Creating heart rate alerts

static func heartRate(ClosedRange&lt;Double>, unit: UnitFrequency) -> Self

Creates a new heart rate alert for the target range.

struct HeartRateRangeAlert

An alert for a range of heart rates.

static func heartRate(zone: Int) -> Self

Creates a new alert for the specified heart rate zone.

struct HeartRateZoneAlert

An alert for a heart rate zone.

### Creating power alerts

static func power(ClosedRange&lt;Double>, unit: UnitPower) -> Self

Creates a new power alert for the target range.

struct PowerRangeAlert

An alert for a range of power values.

static func power(Double, unit: UnitPower) -> Self

Creates an alert for the specified power threshold.

struct PowerThresholdAlert

An alert for a power threshold.

static func power(zone: Int) -> Self

Creates a new alert for the specified power zone.

struct PowerZoneAlert

An alert for a power zone.

### Creating speed alerts

static func speed(ClosedRange&lt;Double>, unit: UnitSpeed, metric: WorkoutAlertMetric) -> Self

Creates a new speed alert for the provided range.

struct SpeedRangeAlert

An alert for a range of speed values.

static func speed(Double, unit: UnitSpeed, metric: WorkoutAlertMetric) -> Self

Creates a new speed threshold alert.

struct SpeedThresholdAlert

An alert for a speed threshold.

### Type Methods

static func power(Double, unit: UnitPower, metric: WorkoutAlertMetric) -> Self

static func power(ClosedRange&lt;Double>, unit: UnitPower, metric: WorkoutAlertMetric) -> Self

## Relationships

### Inherits From

- Equatable
- Hashable
- Sendable

### Conforming Types

- CadenceRangeAlert
- CadenceThresholdAlert
- HeartRateRangeAlert
- HeartRateZoneAlert
- PowerRangeAlert
- PowerThresholdAlert
- PowerZoneAlert
- SpeedRangeAlert
- SpeedThresholdAlert

## See Also

### Custom interval workouts

struct CustomWorkout

A workout that includes a repeating series of work and recovery steps.

struct WorkoutStep

A step in a workout.

struct IntervalBlock

Blocks of work and recovery steps that repeat in a custom workout.

struct IntervalStep

An interval that represents a work or recovery step in a workout.

enum WorkoutGoal

A value that specifies the goal for a workout.


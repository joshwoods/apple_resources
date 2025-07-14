

- HealthKit
- HKWorkoutRouteQueryDescriptor
-  HKWorkoutRouteQueryDescriptor.Results 

Structure

# HKWorkoutRouteQueryDescriptor.Results

An asynchronous sequence that emits data about individual locations from a workout route sample.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct Results
```

## Topics

### Creating an Iterator

struct Iterator

An iterator for accessing individual locations from the workout route.

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Running queries

func results(for: HKHealthStore) -> HKWorkoutRouteQueryDescriptor.Results

Runs a one-shot query that returns an asynchronous sequence of data representing individual locations.


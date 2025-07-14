

- HealthKit
- HKElectrocardiogramQueryDescriptor
-  HKElectrocardiogramQueryDescriptor.Results 

Structure

# HKElectrocardiogramQueryDescriptor.Results

An asynchronous sequence that emits data about individual voltage measurements from an electrocardiogram sample.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct Results
```

## Topics

### Creating an Iterator

struct Iterator

An iterator for accessing individual voltage measurements from the series.

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Running Queries

func results(for: HKHealthStore) -> HKElectrocardiogramQueryDescriptor.Results

Runs a one-shot query that returns an asynchronous sequence of data representing individual heartbeats.


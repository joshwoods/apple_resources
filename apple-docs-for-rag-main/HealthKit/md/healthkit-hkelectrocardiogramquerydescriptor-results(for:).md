

- HealthKit
- HKElectrocardiogramQueryDescriptor
-  results(for:) 

Instance Method

# results(for:)

Runs a one-shot query that returns an asynchronous sequence of data representing individual heartbeats.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
func results(for healthStore: HKHealthStore) -> HKElectrocardiogramQueryDescriptor.Results
```

## Parameters 

`healthStore`  

The access point for HealthKit data.

## See Also

### Running Queries

struct Results

An asynchronous sequence that emits data about individual voltage measurements from an electrocardiogram sample.




- HealthKit
- HKStatisticsQueryDescriptor
-  result(for:) 

Instance Method

# result(for:)

Runs a one-shot query and asynchronously returns a snapshot of the current matching results.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
func result(for healthStore: HKHealthStore) async throws -> HKStatistics?
```

## Parameters 

`healthStore`  

The access point for HealthKit data.


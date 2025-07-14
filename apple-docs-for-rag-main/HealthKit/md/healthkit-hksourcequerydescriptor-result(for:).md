

- HealthKit
- HKSourceQueryDescriptor
-  result(for:) 

Instance Method

# result(for:)

Runs a one-shot query that asynchronously returns a snapshot of all the sources that saved matching data.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
func result(for healthStore: HKHealthStore) async throws -> [HKSource]
```

Available when `Sample` inherits `HKSample`.

## Parameters 

`healthStore`  

The access point for HealthKit data.


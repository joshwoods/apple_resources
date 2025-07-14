

- HealthKit
- HKVerifiableClinicalRecordQueryDescriptor
-  result(for:) 

Instance Method

# result(for:)

Runs a one-shot query that asynchronously reads matching clinical records.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOS

``` source
func result(for healthStore: HKHealthStore) async throws -> [HKVerifiableClinicalRecord]
```

## Parameters 

`healthStore`  

The access point for HealthKit data.


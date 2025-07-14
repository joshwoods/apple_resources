

- HealthKit
- HKAsyncQuery
-  result(for:) 

Instance Method

# result(for:)

Runs a one-shot query and asynchronously returns a snapshot of the current matching results.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
func result(for healthStore: HKHealthStore) async throws -> Self.Output
```

**Required**

## Parameters 

`healthStore`  

The access point for HealthKit data.

## Mentioned in 

Running Queries with Swift Concurrency

## Discussion

The adopting type’s Output associated type specifies the values that this method returns. For example, HKSampleQueryDescriptor returns an array of HKQuantitySample objects.

```
let stepType = HKQuantityType(.stepCount)

let descriptor = HKSampleQueryDescriptor(
    predicates:[.quantitySample(type: stepType)],
    sortDescriptors: [SortDescriptor(\.endDate, order: .reverse)],
    limit: 10)

let results = try await descriptor.result(for: store)
```

## See Also

### Running Queries

associatedtype Output

The type of data that the query returns.

**Required**


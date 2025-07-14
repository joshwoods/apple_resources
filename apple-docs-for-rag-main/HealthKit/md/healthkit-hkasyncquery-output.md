

- HealthKit
- HKAsyncQuery
-  Output 

Associated Type

# Output

The type of data that the query returns.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
associatedtype Output
```

**Required**

## See Also

### Running Queries

func result(for: HKHealthStore) async throws -> Self.Output

Runs a one-shot query and asynchronously returns a snapshot of the current matching results.

**Required**




- HealthKit
- Queries
- HKActivitySummaryQueryDescriptor
-  HKAsyncQuery Implementations 

API Collection

# HKAsyncQuery Implementations

## Topics

### Instance Methods

func result(for: HKHealthStore) async throws -> [HKActivitySummary]

Runs a one-shot query and asynchronously returns a snapshot of the current matching results.


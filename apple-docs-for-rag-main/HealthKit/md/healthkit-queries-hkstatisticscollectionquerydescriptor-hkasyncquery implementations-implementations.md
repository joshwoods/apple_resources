

- HealthKit
- Queries
- HKStatisticsCollectionQueryDescriptor
-  HKAsyncQuery Implementations 

API Collection

# HKAsyncQuery Implementations

## Topics

### Instance Methods

func result(for: HKHealthStore) async throws -> HKStatisticsCollection

Runs a one-shot query and asynchronously returns statistics calculated from the current matching results.


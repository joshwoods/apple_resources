

- HealthKit
- Queries
- HKSampleQueryDescriptor
-  HKAsyncQuery Implementations 

API Collection

# HKAsyncQuery Implementations

## Topics

### Instance Methods

func result(for: HKHealthStore) async throws -> [Sample]

Runs a one-shot query and asynchronously returns a snapshot of the current matching results.


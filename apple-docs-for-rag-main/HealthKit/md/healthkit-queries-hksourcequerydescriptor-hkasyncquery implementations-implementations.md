

- HealthKit
- Queries
- HKSourceQueryDescriptor
-  HKAsyncQuery Implementations 

API Collection

# HKAsyncQuery Implementations

## Topics

### Instance Methods

func result(for: HKHealthStore) async throws -> [HKSource]

Runs a one-shot query that asynchronously returns a snapshot of all the sources that saved matching data.


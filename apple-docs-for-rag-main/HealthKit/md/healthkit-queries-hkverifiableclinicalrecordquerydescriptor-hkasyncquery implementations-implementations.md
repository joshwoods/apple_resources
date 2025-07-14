

- HealthKit
- Queries
- HKVerifiableClinicalRecordQueryDescriptor
-  HKAsyncQuery Implementations 

API Collection

# HKAsyncQuery Implementations

## Topics

### Instance Methods

func result(for: HKHealthStore) async throws -> [HKVerifiableClinicalRecord]

Runs a one-shot query that asynchronously reads matching clinical records.


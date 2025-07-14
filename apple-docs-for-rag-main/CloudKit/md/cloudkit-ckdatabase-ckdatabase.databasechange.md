

- CloudKit
- CKDatabase
-  CKDatabase.DatabaseChange 

Enumeration

# CKDatabase.DatabaseChange

Objects that indicate the type of database change.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
enum DatabaseChange
```

## Topics

### Modifications

struct Modification

A database change that represents the modification of a record zone.

### Deletions

struct Deletion

A database change that represents the deletion of a record zone.

## See Also

### Fetching Changes

func databaseChanges(since: CKServerChangeToken?, resultsLimit: Int?) async throws -> (modifications: [CKDatabase.DatabaseChange.Modification], deletions: [CKDatabase.DatabaseChange.Deletion], changeToken: CKServerChangeToken, moreComing: Bool)

Fetches all modified record zones and returns them to an awaiting caller.

func fetchDatabaseChanges(since: CKServerChangeToken?, resultsLimit: Int?, completionHandler: (Result&lt;(modifications: [CKDatabase.DatabaseChange.Modification], deletions: [CKDatabase.DatabaseChange.Deletion], changeToken: CKServerChangeToken, moreComing: Bool), any Error>) -> Void)

Fetches all modified record zones and delivers them to a completion handler.

func recordZoneChanges(inZoneWith: CKRecordZone.ID, since: CKServerChangeToken?, desiredKeys: [CKRecord.FieldKey]?, resultsLimit: Int?) async throws -> (modificationResultsByID: [CKRecord.ID : Result&lt;CKDatabase.RecordZoneChange.Modification, any Error>], deletions: [CKDatabase.RecordZoneChange.Deletion], changeToken: CKServerChangeToken, moreComing: Bool)

Fetches all modified records from a specific record zone and returns them to an awaiting caller.

func fetchRecordZoneChanges(inZoneWith: CKRecordZone.ID, since: CKServerChangeToken?, desiredKeys: [CKRecord.FieldKey]?, resultsLimit: Int?, completionHandler: (Result&lt;(modificationResultsByID: [CKRecord.ID : Result&lt;CKDatabase.RecordZoneChange.Modification, any Error>], deletions: [CKDatabase.RecordZoneChange.Deletion], changeToken: CKServerChangeToken, moreComing: Bool), any Error>) -> Void)

Fetches all modified records from a specific record zone and delivers them to a completion handler.

enum RecordZoneChange

Objects that indicate the type of record zone change.


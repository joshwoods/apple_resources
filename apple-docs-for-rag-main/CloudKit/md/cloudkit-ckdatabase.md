

- CloudKit
-  CKDatabase 

Class

# CKDatabase

An object that represents a collection of record zones and subscriptions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class CKDatabase
```

## Mentioned in 

Deciding whether CloudKit is right for your app

## Overview

A database takes requests and operations and applies them to the objects it contains, whether that’s record zones, records, or subscriptions. Each of your app’s users has access to the three separate databases:

- A public database that’s accessible to all users of your app.

- A private database that’s accessible only to the user of the current device.

- A shared database that’s accessible only to the user of the current device, which contains records that other iCloud users share with them.

The public database is always available, even when the device doesn’t have an active iCloud account. In this scenario, your app can fetch specific records and perform searches, but it can’t create or modify records. CloudKit requires an iCloud account for writing to the public database so it can identify the authors of any changes. All access to the private and shared databases requires an iCloud account.

You don’t create instances of CKDatabase, nor do you subclass it. Instead, you access the required database using one of your app’s containers. For more information, see CKContainer.

By default, CloudKit executes the methods in this class with a low-priority quality of service (QoS). To use a higher-priority QoS, perform the following:

1.  Create an instance of CKOperation.Configuration and set its qualityOfService property to the preferred value.

2.  Call the databaseʼs configuredWith(configuration:group:body:) method and provide the configuration and a trailing closure.

3.  In the closure, use the provided database to execute the relevant methods at the preferred QoS.

```
func fetchRecords(with ids: [CKRecord.ID]) async throws
    -> [CKRecord.ID: Result] {

    // Get a reference to the user's private database.
    let database = CKContainer.default().privateCloudDatabase

    // Create a configuration with a higher-priority quality of service.
    let config = CKOperation.Configuration()
    config.qualityOfService = .userInitiated

    // Configure the database and execute the fetch.
    return try await database.configuredWith(configuration: config) { db in
        try await db.records(for: ids)
    }
}
```

## Topics

### Configuring Database Requests

func configuredWith&lt;R>(configuration: CKOperation.Configuration?, group: CKOperationGroup?, body: (CKDatabase) async throws -> R) async rethrows -> R

Applies a temporary configuration to the database within the scope of a closure that supports concurrency.

func configuredWith&lt;R>(configuration: CKOperation.Configuration?, group: CKOperationGroup?, body: (CKDatabase) throws -> R) rethrows -> R

Applies a temporary configuration to the database within the scope of a closure.

### Fetching Records

func records(for: [CKRecord.ID], desiredKeys: [CKRecord.FieldKey]?) async throws -> [CKRecord.ID : Result&lt;CKRecord, any Error>]

Fetches the specified records and returns them to an awaiting caller.

func fetch(withRecordIDs: [CKRecord.ID], desiredKeys: [CKRecord.FieldKey]?, completionHandler: (Result&lt;[CKRecord.ID : Result&lt;CKRecord, any Error>], any Error>) -> Void)

Fetches the specified records and delivers them to a completion handler.

func fetch(withRecordID: CKRecord.ID, completionHandler: (CKRecord?, (any Error)?) -> Void)

Fetches a specific record.

### Querying Records

func records(matching: CKQuery, inZoneWith: CKRecordZone.ID?, desiredKeys: [CKRecord.FieldKey]?, resultsLimit: Int) async throws -> (matchResults: [(CKRecord.ID, Result&lt;CKRecord, any Error>)], queryCursor: CKQueryOperation.Cursor?)

Searches for records that match a predicate and returns them to an awaiting caller.

func records(continuingMatchFrom: CKQueryOperation.Cursor, desiredKeys: [CKRecord.FieldKey]?, resultsLimit: Int) async throws -> (matchResults: [(CKRecord.ID, Result&lt;CKRecord, any Error>)], queryCursor: CKQueryOperation.Cursor?)

Retrieves the next batch of records from an existing search and returns them to an awaiting caller.

func fetch(withQuery: CKQuery, inZoneWith: CKRecordZone.ID?, desiredKeys: [CKRecord.FieldKey]?, resultsLimit: Int, completionHandler: (Result&lt;(matchResults: [(CKRecord.ID, Result&lt;CKRecord, any Error>)], queryCursor: CKQueryOperation.Cursor?), any Error>) -> Void)

Searches for records that match a predicate and delivers them to a completion handler.

func fetch(withCursor: CKQueryOperation.Cursor, desiredKeys: [CKRecord.FieldKey]?, resultsLimit: Int, completionHandler: (Result&lt;(matchResults: [(CKRecord.ID, Result&lt;CKRecord, any Error>)], queryCursor: CKQueryOperation.Cursor?), any Error>) -> Void)

Retrieves the next batch of records from an existing search and delivers them to a completion handler.

func perform(CKQuery, inZoneWith: CKRecordZone.ID?, completionHandler: ([CKRecord]?, (any Error)?) -> Void)

Searches for records matching a predicate in the specified record zone.

Deprecated

func records(matching: CKQuery, inZoneWith: CKRecordZone.ID?) async throws -> [CKRecord]

Searches for records in the specified record zone and returns them to an awaiting caller.

Deprecated

### Modifying Records

func modifyRecords(saving: [CKRecord], deleting: [CKRecord.ID], savePolicy: CKModifyRecordsOperation.RecordSavePolicy, atomically: Bool) async throws -> (saveResults: [CKRecord.ID : Result&lt;CKRecord, any Error>], deleteResults: [CKRecord.ID : Result&lt;Void, any Error>])

Modifies the specified records and returns the results to an awaiting caller.

func modifyRecords(saving: [CKRecord], deleting: [CKRecord.ID], savePolicy: CKModifyRecordsOperation.RecordSavePolicy, atomically: Bool, completionHandler: (Result&lt;(saveResults: [CKRecord.ID : Result&lt;CKRecord, any Error>], deleteResults: [CKRecord.ID : Result&lt;Void, any Error>]), any Error>) -> Void)

Modifies the specified records and delivers the results to a completion hander.

enum RecordSavePolicy

Constants that indicate which policy to apply when saving records.

func save(CKRecord, completionHandler: (CKRecord?, (any Error)?) -> Void)

Saves a specific record.

func delete(withRecordID: CKRecord.ID, completionHandler: (CKRecord.ID?, (any Error)?) -> Void)

Deletes a specific record.

### Fetching Record Zones

func recordZones(for: [CKRecordZone.ID]) async throws -> [CKRecordZone.ID : Result&lt;CKRecordZone, any Error>]

Fetches the specified record zones and returns them to an awaiting caller.

func fetch(withRecordZoneIDs: [CKRecordZone.ID], completionHandler: (Result&lt;[CKRecordZone.ID : Result&lt;CKRecordZone, any Error>], any Error>) -> Void)

Fetches the specified record zones and delivers them to a completion handler.

func fetchAllRecordZones(completionHandler: ([CKRecordZone]?, (any Error)?) -> Void)

Fetches all record zones from the current database.

func fetch(withRecordZoneID: CKRecordZone.ID, completionHandler: (CKRecordZone?, (any Error)?) -> Void)

Fetches a specific record zone.

### Modifying Record Zones

func modifyRecordZones(saving: [CKRecordZone], deleting: [CKRecordZone.ID]) async throws -> (saveResults: [CKRecordZone.ID : Result&lt;CKRecordZone, any Error>], deleteResults: [CKRecordZone.ID : Result&lt;Void, any Error>])

Modifies the specified record zones and returns the results to an awaiting caller.

func modifyRecordZones(saving: [CKRecordZone], deleting: [CKRecordZone.ID], completionHandler: (Result&lt;(saveResults: [CKRecordZone.ID : Result&lt;CKRecordZone, any Error>], deleteResults: [CKRecordZone.ID : Result&lt;Void, any Error>]), any Error>) -> Void)

Modifies the specified record zones and delivers the results to a completion handler.

func save(CKRecordZone, completionHandler: (CKRecordZone?, (any Error)?) -> Void)

Saves a specific record zone.

func delete(withRecordZoneID: CKRecordZone.ID, completionHandler: (CKRecordZone.ID?, (any Error)?) -> Void)

Deletes a specific record zone.

### Fetching Subscriptions

func subscriptions(for: [CKSubscription.ID]) async throws -> [CKSubscription.ID : Result&lt;CKSubscription, any Error>]

Fetches the specified subscriptions and returns them to an awaiting caller.

func fetch(withSubscriptionIDs: [CKSubscription.ID], completionHandler: (Result&lt;[CKSubscription.ID : Result&lt;CKSubscription, any Error>], any Error>) -> Void)

Fetches the specified subscriptions and delivers them to a completion handler.

func subscription(for: CKSubscription.ID) async throws -> CKSubscription

Fetches a specific subscription and returns it to an awaiting caller.

func fetch(withSubscriptionID: CKSubscription.ID, completionHandler: (CKSubscription?, (any Error)?) -> Void)

Fetches a specific subscription and delivers it to a completion handler.

func fetchAllSubscriptions(completionHandler: ([CKSubscription]?, (any Error)?) -> Void)

Fetches all subscriptions from the current database.

### Modifying Subscriptions

func modifySubscriptions(saving: [CKSubscription], deleting: [CKSubscription.ID]) async throws -> (saveResults: [CKSubscription.ID : Result&lt;CKSubscription, any Error>], deleteResults: [CKSubscription.ID : Result&lt;Void, any Error>])

Modifies the specified subscriptions and returns the results to an awaiting caller.

func modifySubscriptions(saving: [CKSubscription], deleting: [CKSubscription.ID], completionHandler: (Result&lt;(saveResults: [CKSubscription.ID : Result&lt;CKSubscription, any Error>], deleteResults: [CKSubscription.ID : Result&lt;Void, any Error>]), any Error>) -> Void)

Modifies the specified subscriptions and delivers the results to a completion handler.

func save(CKSubscription, completionHandler: (CKSubscription?, (any Error)?) -> Void)

Saves a specific subscription.

func deleteSubscription(withID: CKSubscription.ID) async throws -> CKSubscription.ID

Deletes a specific subscription and returns the deleted subscription’s identifier to an awaiting caller.

func delete(withSubscriptionID: CKSubscription.ID, completionHandler: (String?, (any Error)?) -> Void)

Deletes a specific subscription and delivers the deleted subscription’s identifier to a completion handler.

### Fetching Changes

func databaseChanges(since: CKServerChangeToken?, resultsLimit: Int?) async throws -> (modifications: [CKDatabase.DatabaseChange.Modification], deletions: [CKDatabase.DatabaseChange.Deletion], changeToken: CKServerChangeToken, moreComing: Bool)

Fetches all modified record zones and returns them to an awaiting caller.

func fetchDatabaseChanges(since: CKServerChangeToken?, resultsLimit: Int?, completionHandler: (Result&lt;(modifications: [CKDatabase.DatabaseChange.Modification], deletions: [CKDatabase.DatabaseChange.Deletion], changeToken: CKServerChangeToken, moreComing: Bool), any Error>) -> Void)

Fetches all modified record zones and delivers them to a completion handler.

enum DatabaseChange

Objects that indicate the type of database change.

func recordZoneChanges(inZoneWith: CKRecordZone.ID, since: CKServerChangeToken?, desiredKeys: [CKRecord.FieldKey]?, resultsLimit: Int?) async throws -> (modificationResultsByID: [CKRecord.ID : Result&lt;CKDatabase.RecordZoneChange.Modification, any Error>], deletions: [CKDatabase.RecordZoneChange.Deletion], changeToken: CKServerChangeToken, moreComing: Bool)

Fetches all modified records from a specific record zone and returns them to an awaiting caller.

func fetchRecordZoneChanges(inZoneWith: CKRecordZone.ID, since: CKServerChangeToken?, desiredKeys: [CKRecord.FieldKey]?, resultsLimit: Int?, completionHandler: (Result&lt;(modificationResultsByID: [CKRecord.ID : Result&lt;CKDatabase.RecordZoneChange.Modification, any Error>], deletions: [CKDatabase.RecordZoneChange.Deletion], changeToken: CKServerChangeToken, moreComing: Bool), any Error>) -> Void)

Fetches all modified records from a specific record zone and delivers them to a completion handler.

enum RecordZoneChange

Objects that indicate the type of record zone change.

### Running Operations

func add(CKDatabaseOperation)

Executes the specified operation in the current database.

### Getting the Database Type

var databaseScope: CKDatabase.Scope

The type of database.

enum Scope

Constants that represent the scope of a database.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Core objects

class CKContainer

A conduit to your app’s databases.

class CKOperationGroup

An explicit association between two or more operations.


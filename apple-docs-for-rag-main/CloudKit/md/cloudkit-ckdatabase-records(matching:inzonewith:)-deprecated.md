

- CloudKit
- CKDatabase
-  records(matching:inZoneWith:) Deprecated

Instance Method

# records(matching:inZoneWith:)

Searches for records in the specified record zone and returns them to an awaiting caller.

iOS 15.0–15.0DeprecatediPadOS 15.0–15.0DeprecatedMac Catalyst 15.0–15.0DeprecatedmacOS 12.0–12.0DeprecatedtvOS 15.0–15.0DeprecatedvisionOSwatchOS 8.0–8.0Deprecated

``` source
func records(
    matching query: CKQuery,
    inZoneWith zoneID: CKRecordZone.ID?
) async throws -> [CKRecord]
```

Deprecated

Use records(matching:inZoneWith:desiredKeys:resultsLimit:) instead.

## Parameters 

`query`  

The query that contains the search parameters. For more information, see CKQuery.

`zoneID`  

The identifier of the record zone to search. If you’re searching a shared database, provide a record zone identifier; otherwise, you can specify `nil` to search all record zones in the database.

## Return Value

An array of records that match the specified query.

## Discussion

For information on a more configurable way to search a database, see CKQueryOperation.

## See Also

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


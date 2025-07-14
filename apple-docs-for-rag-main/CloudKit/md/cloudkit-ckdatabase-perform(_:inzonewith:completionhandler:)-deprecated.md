

- CloudKit
- CKDatabase
-  perform(\_:inZoneWith:completionHandler:) Deprecated

Instance Method

# perform(\_:inZoneWith:completionHandler:)

Searches for records matching a predicate in the specified record zone.

iOS 8.0–15.0DeprecatediPadOS 8.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.10–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
func perform(
    _ query: CKQuery,
    inZoneWith zoneID: CKRecordZone.ID?,
    completionHandler: @escaping ([CKRecord]?, (any Error)?) -> Void
)
```

``` source
func perform(
    _ query: CKQuery,
    inZoneWith zoneID: CKRecordZone.ID?
) async throws -> [CKRecord]
```

Deprecated

renamed to fetch(withQuery:inZoneWith:desiredKeys:resultsLimit:completionHandler:)

## Parameters 

`query`  

The query that contains the search parameters. For more information, see CKQuery.

`zoneID`  

The identifier of the record zone to search. If you’re searching a shared database, provide a record zone identifier; otherwise, you can specify `nil` to search all record zones in the database.

`completionHandler`  

The closure to execute with the search results.

## Discussion

The completion handler takes the following parameters:

- The records that match the specified query, or `nil` if there’s an error.

- An error if a problem occurs, or `nil` if CloudKit completes the search successfully.

For information on a more convenient way to search a database, see records(matching:inZoneWith:desiredKeys:resultsLimit:).

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

func records(matching: CKQuery, inZoneWith: CKRecordZone.ID?) async throws -> [CKRecord]

Searches for records in the specified record zone and returns them to an awaiting caller.

Deprecated


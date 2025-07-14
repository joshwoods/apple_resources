

- CloudKit
- CKDatabase
-  fetch(withRecordIDs:desiredKeys:completionHandler:) 

Instance Method

# fetch(withRecordIDs:desiredKeys:completionHandler:)

Fetches the specified records and delivers them to a completion handler.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
@preconcurrency
func fetch(
    withRecordIDs recordIDs: [CKRecord.ID],
    desiredKeys: [CKRecord.FieldKey]? = nil,
    completionHandler: @escaping (Result], any Error>) -> Void
)
```

## Parameters 

`recordIDs`  

The identifiers of the records to fetch.

`desiredKeys`  

The fields to include on each fetched record. To include all fields, specify `nil`; to fetch only system fields, specify an empty array.

`completionHandler`  

The closure to execute with the fetch results.

## Discussion

The completion handler takes the following parameters:

- A Result that contains either a dictionary of fetched records, or an error if the request fails, such as when the network is unavailable or the device doesn’t have an active iCloud account. When present, the dictionary uses the identifiers you specify in `recordIDs` as its keys. The value of each key is a Result that contains either the corresponding fetched record, or an error that describes why CloudKit can’t provide that record.

If you’re fetching records of different types, make sure that `desiredKeys` is the union of all the fields you require across each distinct record type.

For information on a more configurable way to fetch specific records, see CKFetchRecordsOperation.

## See Also

### Fetching Records

func records(for: [CKRecord.ID], desiredKeys: [CKRecord.FieldKey]?) async throws -> [CKRecord.ID : Result&lt;CKRecord, any Error>]

Fetches the specified records and returns them to an awaiting caller.

func fetch(withRecordID: CKRecord.ID, completionHandler: (CKRecord?, (any Error)?) -> Void)

Fetches a specific record.




- CloudKit
- CKDatabase
-  records(for:desiredKeys:) 

Instance Method

# records(for:desiredKeys:)

Fetches the specified records and returns them to an awaiting caller.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func records(
    for ids: [CKRecord.ID],
    desiredKeys: [CKRecord.FieldKey]? = nil
) async throws -> [CKRecord.ID : Result]
```

## Parameters 

`ids`  

The identifiers of the records to fetch.

`desiredKeys`  

The fields to include on each fetched record. To include all fields, specify `nil`; to fetch only system fields, specify an empty array.

## Return Value

A dictionary that contains the fetched records. The dictionary uses the identifiers you specify in `ids` as its keys. The value of each key is a Result that contains either the corresponding fetched record, or an error that describes why CloudKit can’t provide that record.

## Discussion

If you’re fetching records of different types, make sure that `desiredKeys` is the union of all the fields you require across each distinct record type. This method throws an error if the request fails, such as when the network is unavailable or the device doesn’t have an active iCloud account; otherwise, the returned dictionary includes any individual record errors.

For information on a more configurable way to fetch specific records, see CKFetchRecordsOperation.

## See Also

### Fetching Records

func fetch(withRecordIDs: [CKRecord.ID], desiredKeys: [CKRecord.FieldKey]?, completionHandler: (Result&lt;[CKRecord.ID : Result&lt;CKRecord, any Error>], any Error>) -> Void)

Fetches the specified records and delivers them to a completion handler.

func fetch(withRecordID: CKRecord.ID, completionHandler: (CKRecord?, (any Error)?) -> Void)

Fetches a specific record.


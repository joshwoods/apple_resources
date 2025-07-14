

- CloudKit
- CKDatabase
-  fetch(withRecordID:completionHandler:) 

Instance Method

# fetch(withRecordID:completionHandler:)

Fetches a specific record.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func fetch(
    withRecordID recordID: CKRecord.ID,
    completionHandler: @escaping (CKRecord?, (any Error)?) -> Void
)
```

``` source
func record(for recordID: CKRecord.ID) async throws -> CKRecord
```

## Parameters 

`recordID`  

The identifier of the record to fetch.

`completionHandler`  

The closure to execute with the fetch results.

## Discussion

The completion handler takes the following parameters:

- The requested record, or `nil` if CloudKit can’t provide that record.

- An error if a problem occurs, or `nil` if the fetch completes successfully.

For information on a more convenient way to fetch specific records, see records(for:desiredKeys:).

## See Also

### Fetching Records

func records(for: [CKRecord.ID], desiredKeys: [CKRecord.FieldKey]?) async throws -> [CKRecord.ID : Result&lt;CKRecord, any Error>]

Fetches the specified records and returns them to an awaiting caller.

func fetch(withRecordIDs: [CKRecord.ID], desiredKeys: [CKRecord.FieldKey]?, completionHandler: (Result&lt;[CKRecord.ID : Result&lt;CKRecord, any Error>], any Error>) -> Void)

Fetches the specified records and delivers them to a completion handler.


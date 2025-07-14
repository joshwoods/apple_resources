

- CloudKit
- CKDatabase
-  save(\_:completionHandler:) 

Instance Method

# save(\_:completionHandler:)

Saves a specific record.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func save(
    _ record: CKRecord,
    completionHandler: @escaping (CKRecord?, (any Error)?) -> Void
)
```

``` source
func save(_ record: CKRecord) async throws -> CKRecord
```

## Parameters 

`record`  

The record to save.

`completionHandler`  

The closure to execute after CloudKit saves the record.

## Discussion

The completion handler takes the following parameters:

- The saved record (as it appears on the server), or `nil` if there’s an error.

- An error if a problem occurs, or `nil` if CloudKit successfully saves the record.

The save succeeds only when the specified record is new, or is a more recent version than the one on the server.

For information on a more convenient way to save records, see modifyRecords(saving:deleting:savePolicy:atomically:).

## See Also

### Modifying Records

func modifyRecords(saving: [CKRecord], deleting: [CKRecord.ID], savePolicy: CKModifyRecordsOperation.RecordSavePolicy, atomically: Bool) async throws -> (saveResults: [CKRecord.ID : Result&lt;CKRecord, any Error>], deleteResults: [CKRecord.ID : Result&lt;Void, any Error>])

Modifies the specified records and returns the results to an awaiting caller.

func modifyRecords(saving: [CKRecord], deleting: [CKRecord.ID], savePolicy: CKModifyRecordsOperation.RecordSavePolicy, atomically: Bool, completionHandler: (Result&lt;(saveResults: [CKRecord.ID : Result&lt;CKRecord, any Error>], deleteResults: [CKRecord.ID : Result&lt;Void, any Error>]), any Error>) -> Void)

Modifies the specified records and delivers the results to a completion hander.

enum RecordSavePolicy

Constants that indicate which policy to apply when saving records.

func delete(withRecordID: CKRecord.ID, completionHandler: (CKRecord.ID?, (any Error)?) -> Void)

Deletes a specific record.


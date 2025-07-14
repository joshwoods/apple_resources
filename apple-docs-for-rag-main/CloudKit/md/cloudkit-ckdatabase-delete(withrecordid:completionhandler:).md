

- CloudKit
- CKDatabase
-  delete(withRecordID:completionHandler:) 

Instance Method

# delete(withRecordID:completionHandler:)

Deletes a specific record.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func delete(
    withRecordID recordID: CKRecord.ID,
    completionHandler: @escaping (CKRecord.ID?, (any Error)?) -> Void
)
```

``` source
func deleteRecord(withID recordID: CKRecord.ID) async throws -> CKRecord.ID
```

## Parameters 

`recordID`  

The identifier of the record to delete.

`completionHandler`  

The closure to execute after CloudKit deletes the record.

## Discussion

The completion handler takes the following parameters:

- The identifier of the deleted record, or `nil` if there’s an error.

- An error if a problem occurs, or `nil` if CloudKit successfully deletes the record.

Deleting a record may cause additional deletions if other records in the database reference the deleted record. CloudKit doesn’t provide the identifiers of any additional records it deletes.

For information on a more convenient way to delete records, see modifyRecords(saving:deleting:savePolicy:atomically:).

## See Also

### Modifying Records

func modifyRecords(saving: [CKRecord], deleting: [CKRecord.ID], savePolicy: CKModifyRecordsOperation.RecordSavePolicy, atomically: Bool) async throws -> (saveResults: [CKRecord.ID : Result&lt;CKRecord, any Error>], deleteResults: [CKRecord.ID : Result&lt;Void, any Error>])

Modifies the specified records and returns the results to an awaiting caller.

func modifyRecords(saving: [CKRecord], deleting: [CKRecord.ID], savePolicy: CKModifyRecordsOperation.RecordSavePolicy, atomically: Bool, completionHandler: (Result&lt;(saveResults: [CKRecord.ID : Result&lt;CKRecord, any Error>], deleteResults: [CKRecord.ID : Result&lt;Void, any Error>]), any Error>) -> Void)

Modifies the specified records and delivers the results to a completion hander.

enum RecordSavePolicy

Constants that indicate which policy to apply when saving records.

func save(CKRecord, completionHandler: (CKRecord?, (any Error)?) -> Void)

Saves a specific record.


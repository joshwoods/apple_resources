

- CloudKit
- CKDatabase
-  modifyRecords(saving:deleting:savePolicy:atomically:completionHandler:) 

Instance Method

# modifyRecords(saving:deleting:savePolicy:atomically:completionHandler:)

Modifies the specified records and delivers the results to a completion hander.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
@preconcurrency
func modifyRecords(
    saving recordsToSave: [CKRecord],
    deleting recordIDsToDelete: [CKRecord.ID],
    savePolicy: CKModifyRecordsOperation.RecordSavePolicy = .ifServerRecordUnchanged,
    atomically: Bool = true,
    completionHandler: @escaping (Result], deleteResults: [CKRecord.ID : Result]), any Error>) -> Void
)
```

## Parameters 

`recordsToSave`  

The records to save.

`recordIDsToDelete`  

The identifiers of the records to permanently delete.

`savePolicy`  

The policy to use when modifying existing records. For possible values, see CKModifyRecordsOperation.RecordSavePolicy.

`atomically`  

If true, the entire operation fails if CloudKit can’t modify one or more of the specified records; otherwise, CloudKit reports individual failures in the returned tuple. Atomic changes are only applicable in record zones that have the atomic capability.

`completionHandler`  

The closure to execute after CloudKit processes the changes.

## Discussion

The completion handler takes a single Result parameter that contains either a tuple, or an error if the request fails. For example, when the network is unavailable or the device doesn’t have an active iCloud account, or when `atomically` is true and one or more of the specified changes fail.

When present, the tuple contains the following named elements:

`saveResults`  
A dictionary of saved records. The dictionary uses the identifiers of the records you specify in `recordsToSave` as its keys. The value of each key is a Result that contains either the corresponding modified record (as it appears on the server), or an error that describes why CloudKit can’t modify that record.

`deleteResults`  
A dictionary of deleted records. The dictionary uses the identifiers you specify in `recordIDsToDelete` as its keys. The value of each key is a Result that contains either Void to indicate a successful deletion, or an error that describes why CloudKit can’t delete that record.

Deleting records may cause additional deletions if other records in the database reference the deleted records. CloudKit doesn’t provide the identifiers of any additional records it deletes.

For information on a more configurable way to modify records, see CKModifyRecordsOperation.

## See Also

### Modifying Records

func modifyRecords(saving: [CKRecord], deleting: [CKRecord.ID], savePolicy: CKModifyRecordsOperation.RecordSavePolicy, atomically: Bool) async throws -> (saveResults: [CKRecord.ID : Result&lt;CKRecord, any Error>], deleteResults: [CKRecord.ID : Result&lt;Void, any Error>])

Modifies the specified records and returns the results to an awaiting caller.

enum RecordSavePolicy

Constants that indicate which policy to apply when saving records.

func save(CKRecord, completionHandler: (CKRecord?, (any Error)?) -> Void)

Saves a specific record.

func delete(withRecordID: CKRecord.ID, completionHandler: (CKRecord.ID?, (any Error)?) -> Void)

Deletes a specific record.


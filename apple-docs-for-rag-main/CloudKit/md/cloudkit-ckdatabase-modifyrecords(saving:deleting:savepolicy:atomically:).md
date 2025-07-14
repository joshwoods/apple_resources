

- CloudKit
- CKDatabase
-  modifyRecords(saving:deleting:savePolicy:atomically:) 

Instance Method

# modifyRecords(saving:deleting:savePolicy:atomically:)

Modifies the specified records and returns the results to an awaiting caller.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func modifyRecords(
    saving recordsToSave: [CKRecord],
    deleting recordIDsToDelete: [CKRecord.ID],
    savePolicy: CKModifyRecordsOperation.RecordSavePolicy = .ifServerRecordUnchanged,
    atomically: Bool = true
) async throws -> (saveResults: [CKRecord.ID : Result], deleteResults: [CKRecord.ID : Result])
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

## Return Value

A tuple with the following named elements:

## Discussion

`saveResults`  
A dictionary of saved records. The dictionary uses the identifiers of the records you specify in `recordsToSave` as its keys. The value of each key is a Result that contains either the corresponding modified record (as it appears on the server), or an error that describes why CloudKit can’t modify that record.

`deleteResults`  
A dictionary of deleted records. The dictionary uses the identifiers you specify in `recordIDsToDelete` as its keys. The value of each key is a Result that contains either Void to indicate a successful deletion, or an error that describes why CloudKit can’t delete that record.

## Discussion

Deleting records may cause additional deletions if other records in the database reference the deleted records. CloudKit doesn’t provide the identifiers of any additional records it deletes. This method throws an error if the request fails, such as when the network is unavailable or the device doesn’t have an active iCloud account, or when `atomically` is true and one or more of the specified changes fail; otherwise, the returned tuple includes any individual record errors.

For information on a more configurable way to modify records, see CKModifyRecordsOperation.

## See Also

### Modifying Records

func modifyRecords(saving: [CKRecord], deleting: [CKRecord.ID], savePolicy: CKModifyRecordsOperation.RecordSavePolicy, atomically: Bool, completionHandler: (Result&lt;(saveResults: [CKRecord.ID : Result&lt;CKRecord, any Error>], deleteResults: [CKRecord.ID : Result&lt;Void, any Error>]), any Error>) -> Void)

Modifies the specified records and delivers the results to a completion hander.

enum RecordSavePolicy

Constants that indicate which policy to apply when saving records.

func save(CKRecord, completionHandler: (CKRecord?, (any Error)?) -> Void)

Saves a specific record.

func delete(withRecordID: CKRecord.ID, completionHandler: (CKRecord.ID?, (any Error)?) -> Void)

Deletes a specific record.


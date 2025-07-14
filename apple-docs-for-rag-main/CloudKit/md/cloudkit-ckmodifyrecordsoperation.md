

- CloudKit
-  CKModifyRecordsOperation 

Class

# CKModifyRecordsOperation

An operation that modifies one or more records.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class CKModifyRecordsOperation
```

## Mentioned in 

Encrypting User Data

## Overview

After modifying the fields of a record, use this operation to save those changes to a database. You also use this operation to delete records permanently from a database.

If you’re saving a record that contains a reference to another record, set the reference’s action to indicate if the target record’s deletion should cascade to the saved record. This helps avoid orphaned records in explicit record hierarchies. When creating two new records that have a reference between them, use the same operation to save both records at the same time. During a save operation, CloudKit requires that the target record of the parent reference, if set, exists in the database or is part of the same operation; all other reference fields are exempt from this requirement.

When you save records, the value in the savePolicy property determines how to proceed when CloudKit detects conflicts. Because records can change between the time you fetch them and the time you save them, the save policy determines whether new changes overwrite existing changes. By default, the operation reports an error when there’s a newer version on the server. You can change the default setting to permit your changes to overwrite the server values wholly or partially.

The handlers you assign to monitor progress of the operation execute serially on an internal queue that the operation manages. Your handlers must be capable of executing on a background thread, so any tasks that require access to the main thread must redirect accordingly.

If you assign a completion handler to the completionBlock property of the operation, CloudKit calls it after the operation executes and returns the results. Use the completion handler to perform any housekeeping tasks for the operation, but don’t use it to process the results of the operation. The completion handler you provide should manage any failures of the operation, whether due to an error or an explicit cancellation.

Important

To ensure the speed of fetching and saving records, the server may reject large operations. When this occurs, a block reports the CKError.Code.limitExceeded error. Your app should handle this error, and refactor the operation into multiple smaller batches.

## Topics

### Creating a Modify Record Operation

convenience init(recordsToSave: [CKRecord]?, recordIDsToDelete: [CKRecord.ID]?)

Creates an operation for modifying the specified records.

init()

Creates an empty modify records operation.

### Configuring the Modify Record Operation

var recordsToSave: [CKRecord]?

The records to save to the database.

var recordIDsToDelete: [CKRecord.ID]?

The IDs of the records to delete permanently from the database.

var clientChangeTokenData: Data?

A token that tracks local changes to records.

var isAtomic: Bool

A Boolean value that indicates whether the entire operation fails when CloudKit can’t update one or more records in a record zone.

var savePolicy: CKModifyRecordsOperation.RecordSavePolicy

The policy to use when saving changes to records.

enum RecordSavePolicy

Constants that indicate which policy to apply when saving records.

### Processing the Modify Record Results

var perRecordProgressBlock: ((CKRecord, Double) -> Void)?

The closure to execute with progress information for individual records.

var perRecordCompletionBlock: ((CKRecord, (any Error)?) -> Void)?

The closure to execute when CloudKit saves a record.

Deprecated

var modifyRecordsCompletionBlock: (([CKRecord]?, [CKRecord.ID]?, (any Error)?) -> Void)?

The closure to execute after CloudKit modifies all of the records.

Deprecated

### Instance Properties

var modifyRecordsResultBlock: ((Result&lt;Void, any Error>) -> Void)?

var perRecordDeleteBlock: ((CKRecord.ID, Result&lt;Void, any Error>) -> Void)?

var perRecordSaveBlock: ((CKRecord.ID, Result&lt;CKRecord, any Error>) -> Void)?

## Relationships

### Inherits From

- CKDatabaseOperation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Transactions

class CKModifyRecordZonesOperation

An operation that modifies one or more record zones.


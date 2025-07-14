

- CloudKit
- CKModifyRecordsOperation
-  modifyRecordsCompletionBlock Deprecated

Instance Property

# modifyRecordsCompletionBlock

The closure to execute after CloudKit modifies all of the records.

iOS 8.0–15.0DeprecatediPadOS 8.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.10–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
var modifyRecordsCompletionBlock: (([CKRecord]?, [CKRecord.ID]?, (any Error)?) -> Void)? { get set }
```

Deprecated

Use modifyRecordsResultBlock instead

## Discussion

This property is a closure that returns no value and has the following parameters:

- The records that CloudKit saves.

- The IDs of the records that CloudKit deletes.

- If CloudKit can’t modify any of the records, this parameter provides information about the failure; otherwise, it’s `nil`.

The closure executes only once, and represents your final opportunity to process the operation’s results. It executes after all record progress closures and record completion closures finish. The closure executes serially with respect to the other closures of the operation.

Although this closure executes after the modification of records completes, it executes prior to the indexing of queries for those modified records. Therefore, if a query executes in this completion closure, the results of that query might not include the changes from this operation. Conversely, records that CloudKit fetches in the completion closure are up to date with the changes from the associated operation.

The closure reports an error of type CKError.Code.partialFailure when it modifies only some of the records successfully. The userInfo dictionary of the error contains a CKPartialErrorsByItemIDKey key that has a dictionary as its value. The keys of the dictionary are the IDs of the records that the operation can’t modify, and the corresponding values are errors that contain information about the failures.

If you intend to use this closure to process results, set it before you execute the operation or submit the operation to a queue.

## See Also

### Processing the Modify Record Results

var perRecordProgressBlock: ((CKRecord, Double) -> Void)?

The closure to execute with progress information for individual records.

var perRecordCompletionBlock: ((CKRecord, (any Error)?) -> Void)?

The closure to execute when CloudKit saves a record.

Deprecated


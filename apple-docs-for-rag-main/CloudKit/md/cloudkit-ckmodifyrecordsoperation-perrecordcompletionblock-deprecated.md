

- CloudKit
- CKModifyRecordsOperation
-  perRecordCompletionBlock Deprecated

Instance Property

# perRecordCompletionBlock

The closure to execute when CloudKit saves a record.

iOS 8.0–15.0DeprecatediPadOS 8.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.10–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
var perRecordCompletionBlock: ((CKRecord, (any Error)?) -> Void)? { get set }
```

## Discussion

This property is a closure that returns no value and has the following parameters:

- The record that CloudKit saves.

- If CloudKit can’t save the record, an error that provides information about the failure; otherwise, `nil`.

The closure executes once for each record in the recordsToSave property. Each time the closure executes, it executes serially with respect to the other record completion blocks of the operation.

If you intend to use this closure to process results, set it before you execute the operation or submit the operation to a queue.

## See Also

### Processing the Modify Record Results

var perRecordProgressBlock: ((CKRecord, Double) -> Void)?

The closure to execute with progress information for individual records.

var modifyRecordsCompletionBlock: (([CKRecord]?, [CKRecord.ID]?, (any Error)?) -> Void)?

The closure to execute after CloudKit modifies all of the records.

Deprecated


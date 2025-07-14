

- CloudKit
- CKFetchRecordsOperation
-  perRecordCompletionBlock Deprecated

Instance Property

# perRecordCompletionBlock

The closure to execute when a record becomes available.

iOS 8.0–15.0DeprecatediPadOS 8.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.10–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
var perRecordCompletionBlock: ((CKRecord?, CKRecord.ID?, (any Error)?) -> Void)? { get set }
```

Deprecated

Use perRecordResultBlock instead

## Discussion

This property is a closure that returns no value and has the following parameters:

- The record, or `nil` if CloudKit can’t retrieve the record.

- The ID of the record.

- If CloudKit can’t retrieve the record, an error that provides information about the failure; otherwise, `nil`.

The fetch operation executes this closure once for each record ID in the recordIDs property. Each time the closure executes, it executes serially with respect to the other progress closures of the operation.

If you intend to use this closure to process results, set it before you execute the operation or submit the operation to a queue.

## See Also

### Processing Record Fetch Results

var perRecordProgressBlock: ((CKRecord.ID, Double) -> Void)?

The closure to execute with progress information for individual records.

var fetchRecordsCompletionBlock: (([CKRecord.ID : CKRecord]?, (any Error)?) -> Void)?

The closure to execute after CloudKit retrieves all of the records.

Deprecated


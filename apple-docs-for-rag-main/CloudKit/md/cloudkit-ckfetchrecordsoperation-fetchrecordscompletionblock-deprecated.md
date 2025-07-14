

- CloudKit
- CKFetchRecordsOperation
-  fetchRecordsCompletionBlock Deprecated

Instance Property

# fetchRecordsCompletionBlock

The closure to execute after CloudKit retrieves all of the records.

iOS 8.0–15.0DeprecatediPadOS 8.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.10–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
var fetchRecordsCompletionBlock: (([CKRecord.ID : CKRecord]?, (any Error)?) -> Void)? { get set }
```

Deprecated

Use fetchRecordsResultBlock instead

## Discussion

This property is a closure that returns no value and has the following parameters:

- A dictionary that contains the records that CloudKit retrieves. Each key in the dictionary is a CKRecord.ID object that corresponds to a record you request. The value of each key is the actual CKRecord object that CloudKit returns.

- If CloudKit can’t retrieve any of the records, an error that provides information about the failure; otherwise, `nil`.

The fetch operation executes this closure only once, and it’s your final opportunity to process the results. The closure executes after all of the individual progress closures, but before the operation’s completion closure. The closure executes serially with respect to the other progress closures of the operation.

The closure reports an error of type CKError.Code.partialFailure when it retrieves only some of the records successfully. The userInfo dictionary of the error contains a CKPartialErrorsByItemIDKey key that has a dictionary as its value. The keys of the dictionary are the IDs of the records that the operation can’t retrieve, and the corresponding values are errors that contain information about the failures.

If you intend to use this closure to process results, set it before you execute the operation or submit the operation to a queue.

## See Also

### Processing Record Fetch Results

var perRecordProgressBlock: ((CKRecord.ID, Double) -> Void)?

The closure to execute with progress information for individual records.

var perRecordCompletionBlock: ((CKRecord?, CKRecord.ID?, (any Error)?) -> Void)?

The closure to execute when a record becomes available.

Deprecated


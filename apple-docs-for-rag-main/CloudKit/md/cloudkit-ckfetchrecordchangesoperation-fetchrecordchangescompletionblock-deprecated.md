

- CloudKit
- CKFetchRecordChangesOperation
-  fetchRecordChangesCompletionBlock Deprecated

Instance Property

# fetchRecordChangesCompletionBlock

The block to execute when the system finishes processing all changes.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.12DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
var fetchRecordChangesCompletionBlock: ((CKServerChangeToken?, Data?, (any Error)?) -> Void)? { get set }
```

## Discussion

The block returns no value and takes the following parameters:

`serverChangeToken`  
The new change token from the server. You can store this token locally and use it during subsequent fetch operations to limit the results to records that the system changes after executing the operation.

`clientChangeToken`  
The most recent client change token from the device. If the change token isn’t the most recent change token you provided, the server might not have received the associated changes.

`operationError`  
An error object that contains information about a problem, or `nil` if the system successfully retrieves the changes.

When implementing this block, check the moreComing property of the operation object to ensure that the server was able to deliver all results. If that property is true, you must create another operation object using the value in the `serverChangeToken` parameter to fetch any remaining changes.

The operation object executes this block only once at the conclusion of the operation. It executes after all individual change blocks, but before the operation’s completion block. The block executes serially with respect to the other progress blocks of the operation.

If you intend to use this block to process results, set it before executing the operation or submitting the operation object to a queue.

## See Also

### Processing the Fetch Record Changes Results

var recordChangedBlock: ((CKRecord) -> Void)?

The block to execute with the contents of a changed record.

Deprecated

var recordWithIDWasDeletedBlock: ((CKRecord.ID) -> Void)?

The block to execute with the ID of a deleted record.

Deprecated


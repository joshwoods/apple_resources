

- CloudKit
- CKFetchRecordChangesOperation
-  recordWithIDWasDeletedBlock Deprecated

Instance Property

# recordWithIDWasDeletedBlock

The block to execute with the ID of a deleted record.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.12DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
var recordWithIDWasDeletedBlock: ((CKRecord.ID) -> Void)? { get set }
```

## Discussion

The block returns no value and takes the following parameters:

`recordID`  
The ID of the deleted record.

The operation object executes this block once for each record the server deletes in the record zone after the previous fetch request. Each time the block executes, it executes serially with respect to the other progress blocks of the operation. If there aren’t any deleted records, this block doesn’t execute.

If you intend to use this block to process results, set it before executing the operation or submitting it to a queue.

## See Also

### Processing the Fetch Record Changes Results

var recordChangedBlock: ((CKRecord) -> Void)?

The block to execute with the contents of a changed record.

Deprecated

var fetchRecordChangesCompletionBlock: ((CKServerChangeToken?, Data?, (any Error)?) -> Void)?

The block to execute when the system finishes processing all changes.

Deprecated


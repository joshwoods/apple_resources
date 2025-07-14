

- CloudKit
- CKFetchRecordChangesOperation
-  recordChangedBlock Deprecated

Instance Property

# recordChangedBlock

The block to execute with the contents of a changed record.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.12DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
var recordChangedBlock: ((CKRecord) -> Void)? { get set }
```

## Discussion

The block returns no value and takes the following parameters:

`record`  
The changed record. If you specify a value for the desiredKeys property, the record only contains the fields in the desiredKeys property.

The operation object executes this block once for each record in the zone with changes since the previous fetch request. Each time the block executes, it executes serially with respect to the other progress blocks of the operation. If no records change, the block doesn’t execute.

If you intend to use this block to process results, set it before executing the operation or submitting it to a queue.

## See Also

### Processing the Fetch Record Changes Results

var recordWithIDWasDeletedBlock: ((CKRecord.ID) -> Void)?

The block to execute with the ID of a deleted record.

Deprecated

var fetchRecordChangesCompletionBlock: ((CKServerChangeToken?, Data?, (any Error)?) -> Void)?

The block to execute when the system finishes processing all changes.

Deprecated




- CloudKit
- CKQueryOperation
-  recordFetchedBlock Deprecated

Instance Property

# recordFetchedBlock

The closure to execute when a record becomes available.

iOS 8.0–15.0DeprecatediPadOS 8.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.10–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
var recordFetchedBlock: ((CKRecord) -> Void)? { get set }
```

Deprecated

Use recordMatchedBlock instead, which surfaces per-record errors

## Discussion

The closure returns no value and takes the following parameter:

- A single record that matches the search criteria.

After identifying and sorting the records, the query operation executes this closure once for each of the result’s records. The closure executes serially with respect to all other closures of the operation, so you can expect only one closure at a time to execute for this operation.

Set the property’s value before you execute the operation or submit it to a queue.

Warning

Query indexes update asynchronously so they aren’t always current. If you query for records that you recently changed and don’t allow enough time for those changes to process, the query’s results may be incorrect. The results may not contain the correct records, and the records may be out of order.

## See Also

### Processing the Query Results

var queryCompletionBlock: ((CKQueryOperation.Cursor?, (any Error)?) -> Void)?

The closure to execute after CloudKit retrieves all of the records.

Deprecated


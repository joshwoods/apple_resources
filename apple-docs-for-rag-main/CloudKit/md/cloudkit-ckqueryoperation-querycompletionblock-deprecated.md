

- CloudKit
- CKQueryOperation
-  queryCompletionBlock Deprecated

Instance Property

# queryCompletionBlock

The closure to execute after CloudKit retrieves all of the records.

iOS 8.0–15.0DeprecatediPadOS 8.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.10–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
var queryCompletionBlock: ((CKQueryOperation.Cursor?, (any Error)?) -> Void)? { get set }
```

Deprecated

Use queryResultBlock instead

## Discussion

The closure returns no value and takes the following parameters:

- A cursor that indicates there are more results to fetch, or `nil` if there are no additional results. Use the cursor to create a new query operation when you’re ready to retrieve the next batch of results.

- An error that contains information about a problem, or `nil` if CloudKit retrieves the results successfully.

This closure executes only once, and represents your final opportunity to process the results. It executes after all of the individual record fetch closures. The closure executes serially with respect to the other closures of the operation.

If the number of records that the operation intends to return exceeds resultsLimit, the operation provides a cursor that you can use to retrieve the next batch of results. You must create a separate operation using the cursor to fetch the next batch of results.

Update the value of this property before you execute the operation or submit it to a queue.

## See Also

### Processing the Query Results

var recordFetchedBlock: ((CKRecord) -> Void)?

The closure to execute when a record becomes available.

Deprecated


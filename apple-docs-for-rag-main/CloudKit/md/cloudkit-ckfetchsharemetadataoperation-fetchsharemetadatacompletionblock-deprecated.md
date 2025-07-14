

- CloudKit
- CKFetchShareMetadataOperation
-  fetchShareMetadataCompletionBlock Deprecated

Instance Property

# fetchShareMetadataCompletionBlock

The closure to execute when the operation finishes.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.12–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
var fetchShareMetadataCompletionBlock: (((any Error)?) -> Void)? { get set }
```

Deprecated

Use fetchShareMetadataResultBlock instead

## Discussion

The closure returns no value and takes the following parameter:

- An error that contains information about a problem, or `nil` if CloudKit successfully fetches the metadatas.

The operation executes this closure only once. The closure executes on a background queue, so any tasks that require access to the main queue must dispatch accordingly.

The closure reports an error of type CKError.Code.partialFailure when it can’t fetch some of the metadatas. The `userInfo` dictionary of the error contains a CKPartialErrorsByItemIDKey key that has a dictionary as its value. The keys of the dictionary identify the metadatas that CloudKit can’t fetch, and the corresponding values are errors that contain information about the failures.

Set this property’s value before you execute the operation or submit it to a queue.

## See Also

### Processing the Operation’s Results

var perShareMetadataBlock: ((URL, CKShare.Metadata?, (any Error)?) -> Void)?

The closure to execute as the operation fetches individual shares.

Deprecated


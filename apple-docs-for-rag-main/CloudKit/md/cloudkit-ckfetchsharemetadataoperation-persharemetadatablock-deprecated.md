

- CloudKit
- CKFetchShareMetadataOperation
-  perShareMetadataBlock Deprecated

Instance Property

# perShareMetadataBlock

The closure to execute as the operation fetches individual shares.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.12–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
var perShareMetadataBlock: ((URL, CKShare.Metadata?, (any Error)?) -> Void)? { get set }
```

Deprecated

Use perShareMetadataResultBlock instead

## Discussion

The closure returns no value and takes the following parameters:

- The share’s URL.

- The share metadata, or `nil` if CloudKit can’t fetch the metadata.

- If CloudKit can’t fetch the share metadata, this parameter provides information about the failure; otherwise, it’s `nil`.

The operation executes this closure once for each URL in the shareURLs property. Each time the closure executes, it executes serially with respect to the other closures of the operation.

If you intend to use this closure to process results, set it before you execute the operation or submit the operation to a queue.

## See Also

### Processing the Operation’s Results

var fetchShareMetadataCompletionBlock: (((any Error)?) -> Void)?

The closure to execute when the operation finishes.

Deprecated




- CloudKit
- CKAcceptSharesOperation
-  perShareCompletionBlock Deprecated

Instance Property

# perShareCompletionBlock

The block to execute as CloudKit processes individual shares.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.12–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
var perShareCompletionBlock: ((CKShare.Metadata, CKShare?, (any Error)?) -> Void)? { get set }
```

Deprecated

Use perShareResultBlock instead

## Discussion

The closure returns no value and takes the following parameters:

- The share metadata to process.

- The share, or `nil` if CloudKit can’t process the share metadata.

- If CloudKit can’t process the share metadata, this parameter provides information about the failure; otherwise, it’s `nil`.

The operation executes this closure once for each element in the shareMetadatas property. Each time the closure executes, it executes serially with respect to the other closures of the operation.

If you intend to use this closure to process results, set it before you execute the operation or submit the operation to a queue.

## See Also

### Processing the Share Accept Results

var shareMetadatas: [CKShare.Metadata]?

The share metadatas to process.

var acceptSharesCompletionBlock: (((any Error)?) -> Void)?

The closure to execute when the operation finishes.

Deprecated


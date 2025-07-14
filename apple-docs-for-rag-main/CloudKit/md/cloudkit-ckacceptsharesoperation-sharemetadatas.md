

- CloudKit
- CKAcceptSharesOperation
-  shareMetadatas 

Instance Property

# shareMetadatas

The share metadatas to process.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var shareMetadatas: [CKShare.Metadata]? { get set }
```

## Discussion

Use this property to view or change the metadata of the shares you want to process. If you intend to specify or change the value of this property, do so before you execute the operation or submit it to a queue.

## See Also

### Processing the Share Accept Results

var perShareCompletionBlock: ((CKShare.Metadata, CKShare?, (any Error)?) -> Void)?

The block to execute as CloudKit processes individual shares.

Deprecated

var acceptSharesCompletionBlock: (((any Error)?) -> Void)?

The closure to execute when the operation finishes.

Deprecated


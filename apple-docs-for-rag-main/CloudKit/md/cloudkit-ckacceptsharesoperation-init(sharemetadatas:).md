

- CloudKit
- CKAcceptSharesOperation
-  init(shareMetadatas:) 

Initializer

# init(shareMetadatas:)

Creates an operation for accepting the specified shares.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
convenience init(shareMetadatas: [CKShare.Metadata])
```

## Parameters 

`shareMetadatas`  

The share metadatas to accept. If you specify `nil`, you must assign a value to the shareMetadatas property before you execute the operation.

## Discussion

After initializing the operation, assign a handler to the acceptSharesCompletionBlock property to process the results.

## See Also

### Creating a Share Accept Operation

init()

Creates an operation for accepting shares.




- CloudKit
- CKFetchShareMetadataOperation
-  init(shareURLs:) 

Initializer

# init(shareURLs:)

Creates an operation for fetching the metadata for the specified shares.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
convenience init(shareURLs: [URL])
```

## Parameters 

`shareURLs`  

The URLs of the shares. If you specify `nil`, you must assign a value to the shareURLs property before you execute the operation.

## Discussion

After creating the operation, assign a handler to the fetchShareMetadataCompletionBlock property to process the results.

## See Also

### Creating an Operation

init()

Creates an empty fetch share metadata operation.


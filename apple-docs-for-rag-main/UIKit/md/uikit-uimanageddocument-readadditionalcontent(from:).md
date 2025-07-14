

- UIKit
- UIManagedDocument
-  readAdditionalContent(from:) 

Instance Method

# readAdditionalContent(from:)

Handles reading non-Core Data content in the additional content directory in the document’s file package.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func readAdditionalContent(from absoluteURL: URL) throws
```

## Parameters 

`absoluteURL`  

The URL for the additional content directory in the document’s file package.

## Discussion

You override this method to read non-Core Data content from the additional content directory in the document’s file package.

If you implement this method, it’s invoked automatically by read(from:).

There’s no need to invoke `super`’s implementation.

Handling Errors in Swift

In Swift, this method is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

When overriding this method, use the `throw` statement to throw an `NSError`, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

### Special considerations

Additional content isn’t supported on iCloud.

## See Also

### Customizing read and write operations

func additionalContent(for: URL) throws -> Any

Handles writing non-Core Data content to the additional content directory in the document’s file package.

func writeAdditionalContent(Any, to: URL, originalContentsURL: URL?) throws

Handles writing non-Core Data content to the document’s file package.


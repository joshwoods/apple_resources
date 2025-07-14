

- UIKit
- UIManagedDocument
-  writeAdditionalContent(\_:to:originalContentsURL:) 

Instance Method

# writeAdditionalContent(\_:to:originalContentsURL:)

Handles writing non-Core Data content to the document’s file package.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func writeAdditionalContent(
    _ content: Any,
    to absoluteURL: URL,
    originalContentsURL absoluteOriginalContentsURL: URL?
) throws
```

## Parameters 

`content`  

An object that represents the additional content for the document.

This is the object returned from additionalContent(for:).

`absoluteURL`  

The URL to which to write the additional content.

`absoluteOriginalContentsURL`  

The current URL of the document that’s being saved.

## Discussion

You override this method to perform to write non-Core Data content in the additional content directory in the document’s file package. There are several issues to consider:

- You should typically implement this method only if you also implemented additionalContent(for:).

- Because this method is executed asynchronously, it’s possible that the document’s state may be different from that at which the save operation was initiated. If you need to capture the document state at save time, you should do so in additionalContent(for:).

- If you implement this method, it’s invoked automatically by writeContents(_:andAttributes:safelyTo:for:).

- There’s no need to invoke `super`’s implementation.

Handling Errors in Swift

In Swift, this method is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

When overriding this method, use the `throw` statement to throw an `NSError`, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

### Special considerations

Additional content isn’t supported on iCloud.

## See Also

### Customizing read and write operations

func readAdditionalContent(from: URL) throws

Handles reading non-Core Data content in the additional content directory in the document’s file package.

func additionalContent(for: URL) throws -> Any

Handles writing non-Core Data content to the additional content directory in the document’s file package.


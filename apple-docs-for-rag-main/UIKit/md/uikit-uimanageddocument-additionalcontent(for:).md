

- UIKit
- UIManagedDocument
-  additionalContent(for:) 

Instance Method

# additionalContent(for:)

Handles writing non-Core Data content to the additional content directory in the document’s file package.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func additionalContent(for absoluteURL: URL) throws -> Any
```

## Parameters 

`absoluteURL`  

The URL for the additional content directory in the document’s file package.

## Return Value

An object that contains the additional content for the document at `absoluteURL`, or `nil` if there is a problem.

## Discussion

You override this method to perform to manage non-Core Data content to be stored in the additional content directory in the document’s file package.

If you implement this method, it’s invoked automatically by contents(forType:). The returned object is passed to writeAdditionalContent(_:to:originalContentsURL:).

There’s no need to invoke `super`’s implementation.

Handling Errors in Swift

In Swift, this method is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

When overriding this method, use the `throw` statement to throw an `NSError`, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

### Special considerations

A return value of `nil` indicates an error condition. To avoid generating an exception, you must return a value from this method. If it isn’t always the case that there will be additional content, you should return a sentinel value (for example, an NSNull instance) that you check for in writeAdditionalContent(_:to:originalContentsURL:).

The object returned from this method is passed to writeAdditionalContent(_:to:originalContentsURL:). Because writeAdditionalContent(_:to:originalContentsURL:) is executed on a different thread, you must ensure that the object you return is thread-safe. For example, you might return an NSData object containing an archive of the state you want to capture.

Additional content isn’t supported on iCloud.

## See Also

### Customizing read and write operations

func readAdditionalContent(from: URL) throws

Handles reading non-Core Data content in the additional content directory in the document’s file package.

func writeAdditionalContent(Any, to: URL, originalContentsURL: URL?) throws

Handles writing non-Core Data content to the document’s file package.


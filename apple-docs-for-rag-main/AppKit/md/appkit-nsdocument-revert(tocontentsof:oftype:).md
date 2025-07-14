

- AppKit
- NSDocument
-  revert(toContentsOf:ofType:) 

Instance Method

# revert(toContentsOf:ofType:)

Discards all unsaved document modifications and replaces the document’s contents by reading a file or file package located by a URL of a specified type.

macOS

``` source
@MainActor
func revert(
    toContentsOf url: URL,
    ofType typeName: String
) throws
```

## Parameters 

`url`  

The location from which the document contents are read.

`typeName`  

The string that identifies the document type.

## Discussion

Handling Errors in Swift

In Swift, this method is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

When overriding this method, use the `throw` statement to throw an `NSError`, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.




- AppKit
- NSPersistentDocument
-  revert(toContentsOf:ofType:) 

Instance Method

# revert(toContentsOf:ofType:)

Overridden to clean up the managed object context and controllers during a revert.

macOS

``` source
@MainActor
func revert(
    toContentsOf inAbsoluteURL: URL,
    ofType inTypeName: String
) throws
```

## Parameters 

`inAbsoluteURL`  

An URL object that specifies the location of the file to which to revert.

`inTypeName`  

The type of the document at `inAbsoluteURL`.

## Discussion

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Document Content Management

func read(from: URL, ofType: String) throws

Sets the contents of the receiver by reading from a file of a given type located by a given URL.

func write(to: URL, ofType: String, for: NSDocument.SaveOperationType, originalContentsURL: URL?) throws

Saves changes in the document’s managed object context and saves the document’s persistent store to a given URL.


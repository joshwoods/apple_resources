

- AppKit
- NSPersistentDocument
-  read(from:ofType:) 

Instance Method

# read(from:ofType:)

Sets the contents of the receiver by reading from a file of a given type located by a given URL.

macOS

``` source
nonisolated
func read(
    from absoluteURL: URL,
    ofType typeName: String
) throws
```

## Parameters 

`absoluteURL`  

An URL that specifies the location from which to read the document.

`typeName`  

The document type at `absoluteURL`.

## Discussion

This method sets the URL for the persistent object store associated with the receiver’s managed object context to `absoluteURL`.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

func configurePersistentStoreCoordinator(for: URL, ofType: String, modelConfiguration: String?, storeOptions: [String : Any]?) throws

Configures the receiver’s persistent store coordinator with the appropriate stores for a given URL.

### Document Content Management

func revert(toContentsOf: URL, ofType: String) throws

Overridden to clean up the managed object context and controllers during a revert.

func write(to: URL, ofType: String, for: NSDocument.SaveOperationType, originalContentsURL: URL?) throws

Saves changes in the document’s managed object context and saves the document’s persistent store to a given URL.


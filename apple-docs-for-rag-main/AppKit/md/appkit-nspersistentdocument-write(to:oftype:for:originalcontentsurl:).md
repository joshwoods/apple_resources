

- AppKit
- NSPersistentDocument
-  write(to:ofType:for:originalContentsURL:) 

Instance Method

# write(to:ofType:for:originalContentsURL:)

Saves changes in the document’s managed object context and saves the document’s persistent store to a given URL.

macOS

``` source
nonisolated
func write(
    to absoluteURL: URL,
    ofType typeName: String,
    for saveOperation: NSDocument.SaveOperationType,
    originalContentsURL absoluteOriginalContentsURL: URL?
) throws
```

## Parameters 

`absoluteURL`  

An URL that specifies the new location for the document store. It must not be a relative URL.

`typeName`  

The document type.

`saveOperation`  

The save operation type. See the “Constants” section in NSDocument for possible values.

`absoluteOriginalContentsURL`  

An URL that specifies the location of the original document store.

## Discussion

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

func configurePersistentStoreCoordinator(for: URL, ofType: String, modelConfiguration: String?, storeOptions: [String : Any]?) throws

Configures the receiver’s persistent store coordinator with the appropriate stores for a given URL.

### Document Content Management

func read(from: URL, ofType: String) throws

Sets the contents of the receiver by reading from a file of a given type located by a given URL.

func revert(toContentsOf: URL, ofType: String) throws

Overridden to clean up the managed object context and controllers during a revert.


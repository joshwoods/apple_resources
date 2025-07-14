

- AppKit
- NSDocument
-  duplicate() 

Instance Method

# duplicate()

Creates a new document whose contents are the same as the receiver and returns an error object if unsuccessful.

macOS 10.7+

``` source
@MainActor
func duplicate() throws -> NSDocument
```

## Return Value

The new document if duplication is successful; otherwise `nil`.

## Discussion

The new document returned doesn’t yet have a value to return from fileURL.

The default implementation of this method first uses writeSafely(to:ofType:for:) to write the document’s current contents to a file located in the same directory that is used for the autosaved contents of untitled documents and with the same sort of name, then invokes `[[NSDocumentController sharedDocumentController] duplicateDocumentWithContentsOfURL:newContentsURL copying:NO displayName:aDisplayName error:outError]`.

You can override this method to customize what is done during document duplication, but if your override does not invoke `[NSDocumentController duplicateDocumentWithContentsOfURL:copying:displayName:error:]` you must take care to do things that that method does, especially invoking `[NSDocumentController addDocument:]` and `[NSFileCoordinator addFilePresenter:]`.

Handling Errors in Swift

In Swift, this method is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

When overriding this method, use the `throw` statement to throw an `NSError`, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Duplicating the Document

func duplicate(Any?)

Creates a copy of the receiving document in response to the user choosing Duplicate from the File menu.

func duplicate(withDelegate: Any?, didDuplicate: Selector?, contextInfo: UnsafeMutableRawPointer?)

Creates a new document whose contents are the same as the current document.


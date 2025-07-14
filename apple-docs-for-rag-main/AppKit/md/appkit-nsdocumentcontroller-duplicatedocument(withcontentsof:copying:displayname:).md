

- AppKit
- NSDocumentController
-  duplicateDocument(withContentsOf:copying:displayName:) 

Instance Method

# duplicateDocument(withContentsOf:copying:displayName:)

Creates a new document by reading the contents for the document from another URL, presents its user interface, and returns the document if successful.

macOS 10.7+

``` source
@MainActor
func duplicateDocument(
    withContentsOf url: URL,
    copying duplicateByCopying: Bool,
    displayName displayNameOrNil: String?
) throws -> NSDocument
```

## Parameters 

`url`  

The URL locating the document from which contents of the new document are copied.

`duplicateByCopying`  

If true, the contents located at the passed-in URL are copied into a file located in the directory used for the autosaved contents of untitled documents.

`displayNameOrNil`  

If not `nil` then this value is used to derive a display name for the new document that does not match one that is already in use by an open document.

## Return Value

The newly created NSDocument object, or `nil` if the document could not be created.

## Discussion

The default implementation of this method copies the file if specified, determines the type of the document, calls makeDocument(for:withContentsOf:ofType:) to instantiate it, sends the document `setDisplayName:` to name it if `displayNameOrNil` is not `nil`, calls addDocument(_:) to record its opening, and sends the document makeWindowControllers() and showWindows() messages.

The default implementation of this method uses the file coordination mechanism introduced in OS X v10.7. It passes the document to the `NSFileCoordinator` method addFilePresenter(_:) immediately after calling the addDocument(_:) method. (The balancing invocation of the NSFileCoordinator method removeFilePresenter(_:) is in the NSDocument method close().)

You can override this method to customize how documents are duplicated. It is called by the NSDocument method duplicate(). It may also be called from other places in AppKit.

In most cases, an app does not need to call this method directly.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Creating and Opening Documents

func document(for: URL) -> NSDocument?

Returns, for a given URL, the open document whose file or file package is located by the URL, or `nil` if there is no such open document.

func openDocument(withContentsOf: URL, display: Bool, completionHandler: (NSDocument?, Bool, (any Error)?) -> Void)

Opens a document located by a URL, optionally presents its user interface, and calls the passed-in completion handler.

func openUntitledDocumentAndDisplay(Bool) throws -> NSDocument

Creates a new untitled document, presents its user interface if `displayDocument` is true, and returns the document if successful.

func makeDocument(for: URL?, withContentsOf: URL, ofType: String) throws -> NSDocument

Instantiates a document located by a URL, of a specified type, but by reading the contents for the document from another URL, and returns it if successful.

func makeDocument(withContentsOf: URL, ofType: String) throws -> NSDocument

Instantiates a document located by a URL, of a specified type, and returns it if successful.

func makeUntitledDocument(ofType: String) throws -> NSDocument

Instantiates a new untitled document of the specified type and returns it if successful.

func reopenDocument(for: URL?, withContentsOf: URL, display: Bool, completionHandler: (NSDocument?, Bool, (any Error)?) -> Void)

Reopens a document, optionally located by a URL, by reading the contents for the document from another URL, optionally presents its user interface, and calls the passed-in completion handler.


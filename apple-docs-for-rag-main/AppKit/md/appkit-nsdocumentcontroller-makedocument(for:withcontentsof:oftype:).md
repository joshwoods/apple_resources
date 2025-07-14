

- AppKit
- NSDocumentController
-  makeDocument(for:withContentsOf:ofType:) 

Instance Method

# makeDocument(for:withContentsOf:ofType:)

Instantiates a document located by a URL, of a specified type, but by reading the contents for the document from another URL, and returns it if successful.

macOS

``` source
@MainActor
func makeDocument(
    for urlOrNil: URL?,
    withContentsOf contentsURL: URL,
    ofType typeName: String
) throws -> NSDocument
```

## Parameters 

`urlOrNil`  

The location of the new document object.

`contentsURL`  

The URL of the file that provides the contents for the new document.

`typeName`  

The type of the document.

## Return Value

The newly created NSDocument object, or `nil` if the document could not be created.

## Discussion

The URL is specified by `absoluteDocumentURL`, the type by `typeName`, and the other URL providing the contents by `absoluteDocumentContentsURL`. If not successful, the method returns `nil` after setting `outError` to point to an `NSError` object that encapsulates the reason why the document could not be instantiated. The default implementation of this method calls documentClass(forType:) to find out the class of document to instantiate, allocates a document object, and initializes it by sending it an init(for:withContentsOf:ofType:) message.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Creating and Opening Documents

func document(for: URL) -> NSDocument?

Returns, for a given URL, the open document whose file or file package is located by the URL, or `nil` if there is no such open document.

func duplicateDocument(withContentsOf: URL, copying: Bool, displayName: String?) throws -> NSDocument

Creates a new document by reading the contents for the document from another URL, presents its user interface, and returns the document if successful.

func openDocument(withContentsOf: URL, display: Bool, completionHandler: (NSDocument?, Bool, (any Error)?) -> Void)

Opens a document located by a URL, optionally presents its user interface, and calls the passed-in completion handler.

func openUntitledDocumentAndDisplay(Bool) throws -> NSDocument

Creates a new untitled document, presents its user interface if `displayDocument` is true, and returns the document if successful.

func makeDocument(withContentsOf: URL, ofType: String) throws -> NSDocument

Instantiates a document located by a URL, of a specified type, and returns it if successful.

func makeUntitledDocument(ofType: String) throws -> NSDocument

Instantiates a new untitled document of the specified type and returns it if successful.

func reopenDocument(for: URL?, withContentsOf: URL, display: Bool, completionHandler: (NSDocument?, Bool, (any Error)?) -> Void)

Reopens a document, optionally located by a URL, by reading the contents for the document from another URL, optionally presents its user interface, and calls the passed-in completion handler.


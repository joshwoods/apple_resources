

- AppKit
- NSDocumentController
-  openDocument(withContentsOf:display:completionHandler:) 

Instance Method

# openDocument(withContentsOf:display:completionHandler:)

Opens a document located by a URL, optionally presents its user interface, and calls the passed-in completion handler.

macOS 10.7+

``` source
@MainActor
func openDocument(
    withContentsOf url: URL,
    display displayDocument: Bool,
    completionHandler: @escaping (NSDocument?, Bool, (any Error)?) -> Void
)
```

``` source
@MainActor
func openDocument(
    withContentsOf url: URL,
    display displayDocument: Bool
) async throws -> (NSDocument, Bool)
```

## Parameters 

`url`  

The URL locating the document to open.

`displayDocument`  

If true, displays the document’s user interface.

`completionHandler`  

The completion handler block object passed in to be called at some point in the future, perhaps after the method invocation has returned. The completion handler must be called on the main thread.

The block takes three arguments:

`document`  
The document that was opened, if successful. Otherwise, `nil`.

`documentWasAlreadyOpen`  
Whether the document was already open or being opened when this method was called.

`error`  
If not successful, an `NSError` object that encapsulates the reason why the document could not be opened.

## Discussion

The default implementation of this method checks to see if the document is already open or being opened, and if it is not determines the type of the document, calls makeDocument(withContentsOf:ofType:) to instantiate it, and calls addDocument(_:) to record its opening. If `displayDocument` is true and the document is not already open, the default implementation calls makeWindowControllers() and showWindows(). If the document is already open, the implementation just calls showWindows() if `displayDocument` is true. If the relevant document class returns true when sent canConcurrentlyReadDocuments(ofType:) then the invocation of makeDocument(withContentsOf:ofType:) is done on a thread other than the main one, and when that has returned, the rest of the operation is done on the main thread.

The default implementation of this method uses the file coordination mechanism that was added to the Foundation framework in OS X v10.7. All of the work it does is one big coordinated read, and it passes the document to the `NSFileCoordinator` method addFilePresenter(_:) right after calling addDocument(_:). (The balancing invocation of the `NSFileCoordinator` method removeFilePresenter(_:) is in the `NSDocument` method close().)

You can override this method to customize how documents are opened. Its implementation, however, is somewhat complex, so you should generally investigate overriding one of the methods that it calls instead. However, you can override this method to do additional work before calling the underlying method on `super`. You can also call the underlying method on `super` with a custom completion handler that performs additional work before calling the original completion handler. If you do override this method you should investigate whether you should also override reopenDocument(for:withContentsOf:display:completionHandler:) to apply the same customization. In either case, take care to always call the completion handler on the main thread.

You can call this method to open a document.

### Special Considerations

For backward binary compatibility with OS X v10.6 and earlier, the default implementation of this method calls `[self openDocumentWithContentsOfURL:url display:displayDocument error:&anError]` if that method or the even older openDocumentWithContentsOfFile:display: method is overridden and this one is not, instead of calling makeDocument(withContentsOf:ofType:) and all the rest.

## See Also

### Creating and Opening Documents

func document(for: URL) -> NSDocument?

Returns, for a given URL, the open document whose file or file package is located by the URL, or `nil` if there is no such open document.

func duplicateDocument(withContentsOf: URL, copying: Bool, displayName: String?) throws -> NSDocument

Creates a new document by reading the contents for the document from another URL, presents its user interface, and returns the document if successful.

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


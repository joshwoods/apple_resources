

- UIKit
- UIDocument
-  savingFileType 

Instance Property

# savingFileType

Returns the file type to use for saving a document.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var savingFileType: String? { get }
```

## Return Value

A Uniform Type Identifier (UTI) identifying a document type (for example, PDF or HTML).

## Discussion

The default implementation returns the current file type obtained from the fileType property. The default implementation of the save(to:for:completionHandler:) method appends an extension to the file URL that’s based on the file type. So if you want to move the document to a new type and extension, you can override this method to supply that file type.

## See Also

### Writing document data

func close(completionHandler: ((Bool) -> Void)?)

Asynchronously closes the document after saving any changes.

func contents(forType: String) throws -> Any

Returns the document data to be saved.

func save(to: URL, for: UIDocument.SaveOperation, completionHandler: ((Bool) -> Void)?)

Saves document data to the specified location in the application sandbox.

func writeContents(Any, andAttributes: [AnyHashable : Any]?, safelyTo: URL, for: UIDocument.SaveOperation) throws

Ensures that document data is written safely to a specified location in the application sandbox.

func writeContents(Any, to: URL, for: UIDocument.SaveOperation, originalContentsURL: URL?) throws

Writes the document data to disk at the sandbox location indicated by a file URL.

func fileAttributesToWrite(to: URL, for: UIDocument.SaveOperation) throws -> [AnyHashable : Any]

Returns a dictionary of file attributes to associate with the document file when writing or updating it.

func fileNameExtension(forType: String?, saveOperation: UIDocument.SaveOperation) -> String

Returns a file extension to append to the file URL of the document file being written.


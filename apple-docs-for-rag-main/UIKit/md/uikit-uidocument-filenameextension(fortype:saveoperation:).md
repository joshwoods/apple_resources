

- UIKit
- UIDocument
-  fileNameExtension(forType:saveOperation:) 

Instance Method

# fileNameExtension(forType:saveOperation:)

Returns a file extension to append to the file URL of the document file being written.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func fileNameExtension(
    forType typeName: String?,
    saveOperation: UIDocument.SaveOperation
) -> String
```

## Parameters 

`typeName`  

A Uniform Type Identifier (UTI) that indicates the type of document (for example, PDF or HTML).

`saveOperation`  

A constant that indicates whether the document file is being written the first time or whether it’s being overwritten. See UIDocument.SaveOperation for details.

## Return Value

A string to use as the file extension of the document file.

## Discussion

The default implementation queries Launch Services to obtain the file extension matching the file (document) type. You can override this method to return a file extension that’s different from the default extension. The default implementation of the save(to:for:completionHandler:) method calls this method before it gets the document content and writes the document file to disk.

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

var savingFileType: String?

Returns the file type to use for saving a document.

func fileAttributesToWrite(to: URL, for: UIDocument.SaveOperation) throws -> [AnyHashable : Any]

Returns a dictionary of file attributes to associate with the document file when writing or updating it.


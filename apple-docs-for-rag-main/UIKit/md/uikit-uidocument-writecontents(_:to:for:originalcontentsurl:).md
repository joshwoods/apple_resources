

- UIKit
- UIDocument
-  writeContents(\_:to:for:originalContentsURL:) 

Instance Method

# writeContents(\_:to:for:originalContentsURL:)

Writes the document data to disk at the sandbox location indicated by a file URL.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func writeContents(
    _ contents: Any,
    to url: URL,
    for saveOperation: UIDocument.SaveOperation,
    originalContentsURL: URL?
) throws
```

## Parameters 

`contents`  

The document data to write to disk. Typically, the data is encapsulated by an NSData object (if a flat file) or an FileWrapper object (if a file package).

If the object encapsulating the document data is of some other type, you should override this method or writeContents(_:andAttributes:safelyTo:for:) to perform the actual writing of the data.

`url`  

A file URL specifying the location of the document file in the application sandbox.

`saveOperation`  

A constant that indicates whether the document file is being written the first time or whether it is being overwritten. See UIDocument.SaveOperation for details.

`originalContentsURL`  

A file URL specifying the previous location of the document file (if not `nil`).

## Discussion

This method is called by the writeContents(_:andAttributes:safelyTo:for:) to write the actual file data. It is passed the contents object returned from your contents(forType:) implementation. The default implementation of this method supports NSData or FileWrapper contents by asking the contents object to save itself to the corresponding URL.

If you override this method, you may choose to return a different type of data from contents(forType:) or you may choose to not override contents(forType:) and generate the writable data directly within this method. If you override this method, you should not invoke the superclass implementation.

Handling Errors in Swift

In Swift, this method is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

When overriding this method, use the `throw` statement to throw an `NSError`, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

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

var savingFileType: String?

Returns the file type to use for saving a document.

func fileAttributesToWrite(to: URL, for: UIDocument.SaveOperation) throws -> [AnyHashable : Any]

Returns a dictionary of file attributes to associate with the document file when writing or updating it.

func fileNameExtension(forType: String?, saveOperation: UIDocument.SaveOperation) -> String

Returns a file extension to append to the file URL of the document file being written.


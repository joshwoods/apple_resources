

- UIKit
- UIDocument
-  writeContents(\_:andAttributes:safelyTo:for:) 

Instance Method

# writeContents(\_:andAttributes:safelyTo:for:)

Ensures that document data is written safely to a specified location in the application sandbox.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func writeContents(
    _ contents: Any,
    andAttributes additionalFileAttributes: [AnyHashable : Any]? = nil,
    safelyTo url: URL,
    for saveOperation: UIDocument.SaveOperation
) throws
```

## Parameters 

`contents`  

The document data to write to disk. Typically, the data is encapsulated by an NSData object (if a flat file) or an FileWrapper object (if a file package).

If the object encapsulating the document data is of some other type, you should override this method or writeContents(_:to:for:originalContentsURL:) to perform the actual writing of the data.

`additionalFileAttributes`  

A dictionary of FileManager file attributes to assign to the document file. The default implementation obtains these file attributes by calling fileAttributesToWrite(to:for:).

`url`  

The file URL specifying the location of the document file in the application sandbox.

`saveOperation`  

A constant that indicates whether the document file is being written the first time or whether it is being overwritten. See UIDocument.SaveOperation for details.

## Discussion

This method is called by the save(to:for:completionHandler:) method to save the file data (and associated attributes in the case of an FileWrapper). It creates temporary files and directories as necessary so that successful saves can be completed atomically and failed saves can be rolled back cleanly. This method calls writeContents(_:to:for:originalContentsURL:) to save the `contents` object, passing the location for the new saved file in the `toURL` parameter and the location of the previously existing file in the `originalContentsURL` parameter, if this is an overwrite operation.

If you want to change how file data is saved, you generally override the writeContents(_:to:for:originalContentsURL:) method instead of this method. Additionally, you don’t need to call this method directly unless you are overriding the save(to:for:completionHandler:) method.

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

func writeContents(Any, to: URL, for: UIDocument.SaveOperation, originalContentsURL: URL?) throws

Writes the document data to disk at the sandbox location indicated by a file URL.

var savingFileType: String?

Returns the file type to use for saving a document.

func fileAttributesToWrite(to: URL, for: UIDocument.SaveOperation) throws -> [AnyHashable : Any]

Returns a dictionary of file attributes to associate with the document file when writing or updating it.

func fileNameExtension(forType: String?, saveOperation: UIDocument.SaveOperation) -> String

Returns a file extension to append to the file URL of the document file being written.


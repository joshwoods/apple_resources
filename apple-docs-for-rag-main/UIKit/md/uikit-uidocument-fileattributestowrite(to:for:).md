

- UIKit
- UIDocument
-  fileAttributesToWrite(to:for:) 

Instance Method

# fileAttributesToWrite(to:for:)

Returns a dictionary of file attributes to associate with the document file when writing or updating it.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func fileAttributesToWrite(
    to url: URL,
    for saveOperation: UIDocument.SaveOperation
) throws -> [AnyHashable : Any]
```

## Parameters 

`url`  

A file URL locating the document in the application sandbox.

`saveOperation`  

A constant that indicates whether the document file is being written the first time or whether it’s being overwritten. See UIDocument.SaveOperation for details.

## Return Value

A dictionary of file attributes — for example, level of file protection and creation date. See FileManager for more information about file attributes.

## Discussion

The attributes are associated with a specific file type and save operation. You can override this method to return a dictionary of file attributes that are different than the default file attribute, which for new files is extensionHidden.

The save(to:for:completionHandler:) calls this method before executing asynchronous writing. It passes the dictionary into writeContents(_:andAttributes:safelyTo:for:) when it calls that method to write the document file.

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

func writeContents(Any, to: URL, for: UIDocument.SaveOperation, originalContentsURL: URL?) throws

Writes the document data to disk at the sandbox location indicated by a file URL.

var savingFileType: String?

Returns the file type to use for saving a document.

func fileNameExtension(forType: String?, saveOperation: UIDocument.SaveOperation) -> String

Returns a file extension to append to the file URL of the document file being written.


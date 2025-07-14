

- UIKit
- UIDocument
-  save(to:for:completionHandler:) 

Instance Method

# save(to:for:completionHandler:)

Saves document data to the specified location in the application sandbox.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func save(
    to url: URL,
    for saveOperation: UIDocument.SaveOperation,
    completionHandler: ((Bool) -> Void)? = nil
)
```

``` source
@MainActor
func save(
    to url: URL,
    for saveOperation: UIDocument.SaveOperation
) async -> Bool
```

## Parameters 

`url`  

The file URL identifying the location in the application sandbox to write the document data to. Typically, this is the URL obtained from the fileURL property.

`saveOperation`  

A constant that indicates whether the document file is being written the first time or whether it is being overwritten. See UIDocument.SaveOperation for details.

`completionHandler`  

A block with code that is executed when the save operation concludes. The block returns no value and has one parameter:

`success`  
true if the save operation succeeds, otherwise false.

This block is invoked on the calling queue.

## Discussion

The default implementation of this method first calls the contents(forType:) method synchronously on the calling queue to get the document data to save. Then it calls the writeContents(_:andAttributes:safelyTo:for:) method on a background queue to perform the actual writing of the data to disk.

If you override this method, it’s recommended that you first call the superclass implementation of the method (`super`). If you do not call `super`, you must do two things:

- Call performAsynchronousFileAccess(_:) to put the save operation on a background queue.

- In the block parameter, implement coordinated writing by using the NSFileCoordinator class.

- From within the coordinated write, call writeContents(_:andAttributes:safelyTo:for:).

## See Also

### Writing document data

func close(completionHandler: ((Bool) -> Void)?)

Asynchronously closes the document after saving any changes.

func contents(forType: String) throws -> Any

Returns the document data to be saved.

func writeContents(Any, andAttributes: [AnyHashable : Any]?, safelyTo: URL, for: UIDocument.SaveOperation) throws

Ensures that document data is written safely to a specified location in the application sandbox.

func writeContents(Any, to: URL, for: UIDocument.SaveOperation, originalContentsURL: URL?) throws

Writes the document data to disk at the sandbox location indicated by a file URL.

var savingFileType: String?

Returns the file type to use for saving a document.

func fileAttributesToWrite(to: URL, for: UIDocument.SaveOperation) throws -> [AnyHashable : Any]

Returns a dictionary of file attributes to associate with the document file when writing or updating it.

func fileNameExtension(forType: String?, saveOperation: UIDocument.SaveOperation) -> String

Returns a file extension to append to the file URL of the document file being written.


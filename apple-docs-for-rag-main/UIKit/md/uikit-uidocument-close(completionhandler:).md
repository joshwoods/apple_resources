

- UIKit
- UIDocument
-  close(completionHandler:) 

Instance Method

# close(completionHandler:)

Asynchronously closes the document after saving any changes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func close(completionHandler: ((Bool) -> Void)? = nil)
```

``` source
@MainActor
func close() async -> Bool
```

## Parameters 

`completionHandler`  

A block with code to execute after the save-and-close operation concludes. The block returns no value and has one parameter:

`success`  
true if any save operation succeeds, otherwise false.

The block is invoked on the main queue.

## Discussion

You call this method to begin the sequence of method calls that saves a document safely and asynchronously. The file-system location of the document derives from the fileURL property. After the save operation concludes, the code in `completionHandler` is executed. In this code, you can close the document — for example, by removing the document’s view from the screen. Additionally, if the save operation didn’t succeed (`success` is false), you can respond in an appropriate manner.

You typically wouldn’t override this method. The default implementation calls the autosave(completionHandler:) method.

## See Also

### Writing document data

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

func fileNameExtension(forType: String?, saveOperation: UIDocument.SaveOperation) -> String

Returns a file extension to append to the file URL of the document file being written.




- AppKit
- NSDocument
-  canAsynchronouslyWrite(to:ofType:for:) 

Instance Method

# canAsynchronouslyWrite(to:ofType:for:)

Returns whether the receiver can concurrently write to a file or file package located by a URL, that is formatted for a specific type, for a specific kind of save operation.

macOS 10.7+

``` source
@MainActor
func canAsynchronouslyWrite(
    to url: URL,
    ofType typeName: String,
    for saveOperation: NSDocument.SaveOperationType
) -> Bool
```

## Parameters 

`url`  

The location of the file or package to which the document is written.

`typeName`  

The string that identifies the document type.

`saveOperation`  

The type of save operation.

## Return Value

false by default; subclasses can override to return true, thereby enabling asynchronous writing.

## Discussion

The default implementation of this method returns false. You are strongly encouraged to override it and make it return true, after making sure your overrides of document writing methods can be safely invoked on a non-main thread, and making sure that the unblockUserInteraction() method is invoked at some appropriate time during writing.

## See Also

### Writing the Document’s Content

func unblockUserInteraction()

Unblocks the main thread during asynchronous saving.

func write(to: URL, ofType: String) throws

Writes the contents of the document to a file or file package located by a URL, that is formatted to a specified type.

func writeSafely(to: URL, ofType: String, for: NSDocument.SaveOperationType) throws

Writes the contents of the document to a file or file package located by a URL.

func fileWrapper(ofType: String) throws -> FileWrapper

Creates and returns a file wrapper that contains the contents of the document, formatted to the specified type.

func data(ofType: String) throws -> Data

Creates and returns a data object that contains the contents of the document, formatted to a specified type.

func write(to: URL, ofType: String, for: NSDocument.SaveOperationType, originalContentsURL: URL?) throws

Writes the contents of the document to a file or file package located by a URL.

func save(to: URL, ofType: String, for: NSDocument.SaveOperationType, delegate: Any?, didSave: Selector?, contextInfo: UnsafeMutableRawPointer?)

Saves the contents of the document to a file or file package located by a URL, that is formatted to a specified type, for a particular kind of save operation.

func save(to: URL, ofType: String, for: NSDocument.SaveOperationType, completionHandler: ((any Error)?) -> Void)

Saves the contents of the document to a file or file package located by a URL, that is formatted to a specified type, for a particular kind of save operation, and invokes the passed-in completion handler.

func fileAttributesToWrite(to: URL, ofType: String, for: NSDocument.SaveOperationType, originalContentsURL: URL?) throws -> [String : Any]

Returns the attributes to write to the file or file package at the specified URL, and targeting the specified type of save operation.

enum SaveOperationType

Constants for specifying the type of document-save operation to perform.


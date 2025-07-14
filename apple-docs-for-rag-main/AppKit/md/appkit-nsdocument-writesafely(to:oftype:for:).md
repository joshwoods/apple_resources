

- AppKit
- NSDocument
-  writeSafely(to:ofType:for:) 

Instance Method

# writeSafely(to:ofType:for:)

Writes the contents of the document to a file or file package located by a URL.

macOS

``` source
nonisolated
func writeSafely(
    to url: URL,
    ofType typeName: String,
    for saveOperation: NSDocument.SaveOperationType
) throws
```

## Parameters 

`url`  

The location to which the document contents are written.

`typeName`  

The string that identifies the document type.

`saveOperation`  

The type of save operation.

## Discussion

The default implementation of this method invokes write(to:ofType:for:originalContentsURL:). It also invokes fileAttributesToWrite(to:ofType:for:originalContentsURL:) and writes the returned attributes, if any, to the file. It may copy some attributes from the old on-disk revision of the document at the same time, if applicable.

This method is responsible for doing document writing in a way that minimizes the danger of leaving the disk to which writing is being done in an inconsistent state in the event of an app crash, system crash, hardware failure, power outage, and so on. If you override this method, be sure to invoke the superclass implementation.

For `NSSaveOperation`, the default implementation of this method uses the value in the keepBackupFile property to determine whether or not the old on-disk revision of the document, if there was one, should be preserved after being renamed.

For backward binary compatibility with OS X v10.3 and earlier, the default implementation of this method instead invokes writeWithBackupToFile:ofType:saveOperation: if that method is is overridden and the URL uses the `file:` scheme. The save operation in this case is never `NSAutosaveOperation`; `NSSaveToOperation` is used instead.

Handling Errors in Swift

In Swift, this method is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

When overriding this method, use the `throw` statement to throw an `NSError`, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Writing the Document’s Content

func canAsynchronouslyWrite(to: URL, ofType: String, for: NSDocument.SaveOperationType) -> Bool

Returns whether the receiver can concurrently write to a file or file package located by a URL, that is formatted for a specific type, for a specific kind of save operation.

func unblockUserInteraction()

Unblocks the main thread during asynchronous saving.

func write(to: URL, ofType: String) throws

Writes the contents of the document to a file or file package located by a URL, that is formatted to a specified type.

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


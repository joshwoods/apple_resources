

- AppKit
- NSDocument
-  NSDocument.SaveOperationType 

Enumeration

# NSDocument.SaveOperationType

Constants for specifying the type of document-save operation to perform.

macOS

``` source
enum SaveOperationType
```

## Overview

These values are used with method parameters of type NSDocument.SaveOperationType. Depending on the method, the save operation type can affect the title of the Save dialog and can affect which files are displayed in the dialog.

## Topics

### Constants

case saveOperation

An operation that overwrites a document’s file or file package with the document’s contents.

case saveAsOperation

An operation that writes the document’s contents to a new location and updates the document to point to that location

case saveToOperation

An operation that writes a copy of the document’s contents to the specified location, without changing the original document’s location.

case autosaveElsewhereOperation

An operation that writes an autosave version of the file to a different location.

case autosaveInPlaceOperation

An operation that overwrites the document’s current contents with autosave data.

case autosaveAsOperation

An operation that writes a document’s contents to a new file or file package even though the user has not explicitly requested it, then changes the document’s current location to point to the just-written file or file package.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Writing the Document’s Content

func canAsynchronouslyWrite(to: URL, ofType: String, for: NSDocument.SaveOperationType) -> Bool

Returns whether the receiver can concurrently write to a file or file package located by a URL, that is formatted for a specific type, for a specific kind of save operation.

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




- AppKit
- NSDocument
-  updateChangeCount(withToken:for:) 

Instance Method

# updateChangeCount(withToken:for:)

Updates the document’s change count settings after a successful save operation.

macOS 10.7+

``` source
@MainActor
func updateChangeCount(
    withToken changeCountToken: Any,
    for saveOperation: NSDocument.SaveOperationType
)
```

## Parameters 

`changeCountToken`  

An object encapsulating the document changes, returned from changeCountToken(for:).

`saveOperation`  

The type of save operation.

## Discussion

This method updates the values in the isDocumentEdited and hasUnautosavedChanges properties. For example, save(to:ofType:for:completionHandler:) invokes this method, on the main thread, when it is done saving. The default implementation of this method also sends all of the document’s window controllers setDocumentEdited(_:) messages when appropriate.

## See Also

### Updating the Document Change Count

func updateChangeCount(NSDocument.ChangeType)

Updates the receiver’s change count according to the given change type.

enum ChangeType

Values that indicate a document’s edit status.

func changeCountToken(for: NSDocument.SaveOperationType) -> Any

Returns an object that encapsulates the current record of document changes at the beginning of a save operation.


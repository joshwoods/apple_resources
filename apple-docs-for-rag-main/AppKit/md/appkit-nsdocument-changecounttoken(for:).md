

- AppKit
- NSDocument
-  changeCountToken(for:) 

Instance Method

# changeCountToken(for:)

Returns an object that encapsulates the current record of document changes at the beginning of a save operation.

macOS 10.7+

``` source
@MainActor
func changeCountToken(for saveOperation: NSDocument.SaveOperationType) -> Any
```

## Parameters 

`saveOperation`  

The type of save operation.

## Return Value

An object encapsulating the document changes.

## Discussion

The returned object is meant to be passed to updateChangeCount(withToken:for:) at the end of the save operation. For example, save(to:ofType:for:completionHandler:) invokes this method, on the main thread, before it does any actual saving. This method facilitates asynchronous saving, during which a user can change a document while it is being saved.

## See Also

### Updating the Document Change Count

func updateChangeCount(withToken: Any, for: NSDocument.SaveOperationType)

Updates the document’s change count settings after a successful save operation.

func updateChangeCount(NSDocument.ChangeType)

Updates the receiver’s change count according to the given change type.

enum ChangeType

Values that indicate a document’s edit status.


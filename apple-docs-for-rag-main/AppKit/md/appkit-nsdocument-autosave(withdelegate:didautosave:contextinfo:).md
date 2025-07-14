

- AppKit
- NSDocument
-  autosave(withDelegate:didAutosave:contextInfo:) 

Instance Method

# autosave(withDelegate:didAutosave:contextInfo:)

Autosaves the document’s contents to an appropriate location in the file system.

macOS

``` source
@MainActor
func autosave(
    withDelegate delegate: Any?,
    didAutosave didAutosaveSelector: Selector?,
    contextInfo: UnsafeMutableRawPointer?
)
```

## Parameters 

`delegate`  

The delegate to which the selector message is sent.

`didAutosaveSelector`  

The selector of the message sent to the delegate.

`contextInfo`  

Object passed with the callback to provide any additional context information.

## Discussion

After autosaving, sends the message selected by `didAutosaveSelector` to the delegate, with `contextInfo` as the last argument. The method selected by `didAutosaveSelector` must have the same signature as:

```
- (void)document:(NSDocument *)document didAutosave:(BOOL)didAutosaveSuccessfully contextInfo:(void *)contextInfo
```

If an error occurs while autosaving, the method reports it to the user before sending the delegate a `succeeded:NO` message.

## See Also

### Related Documentation

var autosavedContentsFileURL: URL?

The location of the most recently autosaved document contents.

### Autosaving the Document

func checkAutosavingSafety() throws

Returns a Boolean value that indicates whether it is safe to autosave document changes.

var hasUnautosavedChanges: Bool

A Boolean value that indicates whether the document has changes that have not been autosaved.

func scheduleAutosaving()

Schedules periodic autosaving for the purpose of crash protection.

func autosave(withImplicitCancellability: Bool, completionHandler: ((any Error)?) -> Void)

Autosaves the document’s contents to an appropriate file-system location, as needed.

var backupFileURL: URL?

The URL for the document’s backup file that was created during an autosave operation.


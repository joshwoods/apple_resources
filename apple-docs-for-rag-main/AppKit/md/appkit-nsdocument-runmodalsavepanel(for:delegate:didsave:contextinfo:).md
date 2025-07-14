

- AppKit
- NSDocument
-  runModalSavePanel(for:delegate:didSave:contextInfo:) 

Instance Method

# runModalSavePanel(for:delegate:didSave:contextInfo:)

Presents a modal Save panel to the user, then tries to save the document if the user approves the operation.

macOS

``` source
@MainActor
func runModalSavePanel(
    for saveOperation: NSDocument.SaveOperationType,
    delegate: Any?,
    didSave didSaveSelector: Selector?,
    contextInfo: UnsafeMutableRawPointer?
)
```

## Parameters 

`saveOperation`  

The type of save operation.

`delegate`  

The delegate to which the selector message is sent.

`didSaveSelector`  

The selector of the message sent to the delegate.

`contextInfo`  

Object passed with the callback to provide any additional context information.

## Discussion

When saving is completed, regardless of success or failure, or has been canceled, sends the message selected by `didSaveSelector` to the `delegate`, with `contextInfo` as the last argument. The method selected by `didSaveSelector` must have the same signature as:

```
- (void)document:(NSDocument *)doc didSave:(BOOL)didSave contextInfo:(void  *)contextInfo
```

Invoked from save(withDelegate:didSave:contextInfo:), and from the saveAs(_:) and saveTo(_:) action methods. The default implementation of this method first makes sure that any editor registered using the Cocoa Bindings NSEditorRegistration informal protocol has committed its changes, then creates a Save panel, adds a standard file format accessory view (if there is more than one file type for the user to choose from and shouldRunSavePanelWithAccessoryView returns true), sets various attributes of the panel, invokes prepareSavePanel(_:) to provide an opportunity for customization, then presents the panel. If the user approves the panel, the default implementation sends the message save(to:ofType:for:delegate:didSave:contextInfo:).

For backward binary compatibility with Mac OS v10.3 and earlier, the default implementation of this method instead invokes the deprecated saveToFile:saveOperation:delegate:didSaveSelector:contextInfo: if it is overridden, even if the user cancels the panel.

## See Also

### Presenting a Save Panel

func prepareSavePanel(NSSavePanel) -> Bool

Tells the document to customize the specified Save panel.

var shouldRunSavePanelWithAccessoryView: Bool

A Boolean value that indicates whether the document’s Save panel displays a list of supported writable document types.

Deprecated

var fileTypeFromLastRunSavePanel: String?

The file type that was last selected in the Save panel.

var fileNameExtensionWasHiddenInLastRunSavePanel: Bool

A Boolean value that indicates whether the user chose to hide the document’s filename extension.


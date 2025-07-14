

- AppKit
- NSDocument
-  prepareSavePanel(\_:) 

Instance Method

# prepareSavePanel(\_:)

Tells the document to customize the specified Save panel.

macOS

``` source
@MainActor
func prepareSavePanel(_ savePanel: NSSavePanel) -> Bool
```

## Parameters 

`savePanel`  

The Save panel.

## Return Value

true if successfully prepared; otherwise, false.

## Discussion

The default implementation is empty and returns true.

## See Also

### Presenting a Save Panel

func runModalSavePanel(for: NSDocument.SaveOperationType, delegate: Any?, didSave: Selector?, contextInfo: UnsafeMutableRawPointer?)

Presents a modal Save panel to the user, then tries to save the document if the user approves the operation.

var shouldRunSavePanelWithAccessoryView: Bool

A Boolean value that indicates whether the document’s Save panel displays a list of supported writable document types.

Deprecated

var fileTypeFromLastRunSavePanel: String?

The file type that was last selected in the Save panel.

var fileNameExtensionWasHiddenInLastRunSavePanel: Bool

A Boolean value that indicates whether the user chose to hide the document’s filename extension.


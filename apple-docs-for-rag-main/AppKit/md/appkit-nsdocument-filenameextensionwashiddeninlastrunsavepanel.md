

- AppKit
- NSDocument
-  fileNameExtensionWasHiddenInLastRunSavePanel 

Instance Property

# fileNameExtensionWasHiddenInLastRunSavePanel

A Boolean value that indicates whether the user chose to hide the document’s filename extension.

macOS

``` source
nonisolated
var fileNameExtensionWasHiddenInLastRunSavePanel: Bool { get }
```

## Return Value

true if a Save panel was presented and the user chose to hide the extension; otherwise, false.

## Discussion

The Save panel includes an option to hide a document’s filename extension. If the user selects this option, AppKit sets the value of this property to true; otherwise, the value is false.

## See Also

### Presenting a Save Panel

func runModalSavePanel(for: NSDocument.SaveOperationType, delegate: Any?, didSave: Selector?, contextInfo: UnsafeMutableRawPointer?)

Presents a modal Save panel to the user, then tries to save the document if the user approves the operation.

func prepareSavePanel(NSSavePanel) -> Bool

Tells the document to customize the specified Save panel.

var shouldRunSavePanelWithAccessoryView: Bool

A Boolean value that indicates whether the document’s Save panel displays a list of supported writable document types.

Deprecated

var fileTypeFromLastRunSavePanel: String?

The file type that was last selected in the Save panel.


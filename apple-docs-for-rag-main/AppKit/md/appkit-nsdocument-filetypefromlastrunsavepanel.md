

- AppKit
- NSDocument
-  fileTypeFromLastRunSavePanel 

Instance Property

# fileTypeFromLastRunSavePanel

The file type that was last selected in the Save panel.

macOS

``` source
nonisolated
var fileTypeFromLastRunSavePanel: String? { get }
```

## Discussion

This type is primarily used by the save(_:), saveAs(_:), and saveTo(_:) methods to determine the type the user chose after the Save panel has been run. The string corresponds to the name of the document type as it is specified in the app’s `Info.plist` file.

## See Also

### Presenting a Save Panel

func runModalSavePanel(for: NSDocument.SaveOperationType, delegate: Any?, didSave: Selector?, contextInfo: UnsafeMutableRawPointer?)

Presents a modal Save panel to the user, then tries to save the document if the user approves the operation.

func prepareSavePanel(NSSavePanel) -> Bool

Tells the document to customize the specified Save panel.

var shouldRunSavePanelWithAccessoryView: Bool

A Boolean value that indicates whether the document’s Save panel displays a list of supported writable document types.

Deprecated

var fileNameExtensionWasHiddenInLastRunSavePanel: Bool

A Boolean value that indicates whether the user chose to hide the document’s filename extension.


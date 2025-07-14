

- AppKit
- NSDocument
-  shouldRunSavePanelWithAccessoryView Deprecated

Instance Property

# shouldRunSavePanelWithAccessoryView

A Boolean value that indicates whether the document’s Save panel displays a list of supported writable document types.

macOS 10.0–15.4Deprecated

``` source
@MainActor
var shouldRunSavePanelWithAccessoryView: Bool { get }
```

## Discussion

When the value of this property is true, the document includes a pop-up menu of supported writable document types when it displays the Save panel. The default value of this property is true. Subclasses can override this property to provide a different value. For example, you might provide the following implementation:

```
- (BOOL)shouldRunSavePanelWithAccessoryView {
    return [self fileURL] == nil;
}
```

## See Also

### Presenting a Save Panel

func runModalSavePanel(for: NSDocument.SaveOperationType, delegate: Any?, didSave: Selector?, contextInfo: UnsafeMutableRawPointer?)

Presents a modal Save panel to the user, then tries to save the document if the user approves the operation.

func prepareSavePanel(NSSavePanel) -> Bool

Tells the document to customize the specified Save panel.

var fileTypeFromLastRunSavePanel: String?

The file type that was last selected in the Save panel.

var fileNameExtensionWasHiddenInLastRunSavePanel: Bool

A Boolean value that indicates whether the user chose to hide the document’s filename extension.


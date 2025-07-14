

- AppKit
- NSOpenSavePanelDelegate
-  panelSelectionDidChange(\_:) 

Instance Method

# panelSelectionDidChange(\_:)

Tells the delegate that the user changed the selection in the specified Save panel.

macOS

``` source
@MainActor
optional func panelSelectionDidChange(_ sender: Any?)
```

## Parameters 

`sender`  

The panel whose selection changed.

## See Also

### Responding to Panel Changes

func panel(Any, didChangeToDirectoryURL: URL?)

Tells the delegate that the user changed the selected directory to the directory located at the specified URL.

func panel(Any, willExpand: Bool)

Tells the delegate that the Save panel is about to expand or collapse because the user clicked the disclosure triangle that displays or hides the file browser.


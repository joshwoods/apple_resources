

- AppKit
- NSOpenSavePanelDelegate
-  panel(\_:willExpand:) 

Instance Method

# panel(\_:willExpand:)

Tells the delegate that the Save panel is about to expand or collapse because the user clicked the disclosure triangle that displays or hides the file browser.

macOS

``` source
@MainActor
optional func panel(
    _ sender: Any,
    willExpand expanding: Bool
)
```

## Parameters 

`sender`  

The panel that is about to expand or collapse.

`expanding`  

true specifies that the panel is expanding; false specifies that it is collapsing.

## See Also

### Responding to Panel Changes

func panelSelectionDidChange(Any?)

Tells the delegate that the user changed the selection in the specified Save panel.

func panel(Any, didChangeToDirectoryURL: URL?)

Tells the delegate that the user changed the selected directory to the directory located at the specified URL.


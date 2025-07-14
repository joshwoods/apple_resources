

- AppKit
- NSOpenSavePanelDelegate
-  panel(\_:didChangeToDirectoryURL:) 

Instance Method

# panel(\_:didChangeToDirectoryURL:)

Tells the delegate that the user changed the selected directory to the directory located at the specified URL.

macOS 10.6+

``` source
@MainActor
optional func panel(
    _ sender: Any,
    didChangeToDirectoryURL url: URL?
)
```

## Parameters 

`sender`  

The panel whose directory changed.

`url`  

The URL of the new directory, or `nil` if it can’t be represented by an NSURL object.

## See Also

### Responding to Panel Changes

func panelSelectionDidChange(Any?)

Tells the delegate that the user changed the selection in the specified Save panel.

func panel(Any, willExpand: Bool)

Tells the delegate that the Save panel is about to expand or collapse because the user clicked the disclosure triangle that displays or hides the file browser.


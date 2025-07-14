

- AppKit
- NSPrintPanel
-  runModal() 

Instance Method

# runModal()

Displays the Print panel and begins the modal loop.

macOS

``` source
@MainActor
func runModal() -> Int
```

## Return Value

`NSCancelButton` if the user clicks the Cancel button; otherwise `NSOKButton`.

## Discussion

This method uses the printing information associated with the current printing operation.

## See Also

### Related Documentation

var printInfo: NSPrintInfo

The printing information associated with the print operation.

### Running the Panel

func beginSheet(using: NSPrintInfo, on: NSWindow, completionHandler: ((NSPrintPanel.Result) -> Void)?)

func beginSheet(with: NSPrintInfo, modalFor: NSWindow, delegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer?)

Displays a Print panel sheet and runs it modally for the specified window.

Deprecated

func runModal(with: NSPrintInfo) -> Int

Displays the Print panel and runs the modal loop using the specified printing information.


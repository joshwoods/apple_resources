

- AppKit
- NSPrintPanel
-  runModal(with:) 

Instance Method

# runModal(with:)

Displays the Print panel and runs the modal loop using the specified printing information.

macOS 10.5+

``` source
@MainActor
func runModal(with printInfo: NSPrintInfo) -> Int
```

## Parameters 

`printInfo`  

The printing information to use while displaying the Print panel.

## Return Value

`NSCancelButton` if the user clicks the Cancel button; otherwise `NSOKButton`.

## See Also

### Running the Panel

func beginSheet(using: NSPrintInfo, on: NSWindow, completionHandler: ((NSPrintPanel.Result) -> Void)?)

func beginSheet(with: NSPrintInfo, modalFor: NSWindow, delegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer?)

Displays a Print panel sheet and runs it modally for the specified window.

Deprecated

func runModal() -> Int

Displays the Print panel and begins the modal loop.


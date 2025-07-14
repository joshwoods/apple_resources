

- AppKit
- NSPageLayout
-  runModal() 

Instance Method

# runModal()

Displays the page layout panel and begins the modal loop using the shared print info object.

macOS

``` source
@MainActor
func runModal() -> Int
```

## Return Value

`NSCancelButton` if the user clicks the Cancel button; otherwise, `NSOKButton`.

## Discussion

The receiver’s values are recorded in the shared `NSPrintInfo` object.

## See Also

### Running the page setup dialog

func beginSheet(using: NSPrintInfo, on: NSWindow, completionHandler: ((NSPageLayout.Result) -> Void)?)

func beginSheet(with: NSPrintInfo, modalFor: NSWindow, delegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer?)

Presents a page setup sheet for the specified print info object, document-modal relative to the specified window.

Deprecated

func runModal(with: NSPrintInfo) -> Int

Displays the page layout panel and begins the modal loop using the specified print info object.




- AppKit
- NSPageLayout
-  runModal(with:) 

Instance Method

# runModal(with:)

Displays the page layout panel and begins the modal loop using the specified print info object.

macOS

``` source
@MainActor
func runModal(with printInfo: NSPrintInfo) -> Int
```

## Parameters 

`printInfo`  

The `NSPrintInfo` object to use.

## Return Value

`NSCancelButton` if the user clicks the Cancel button; otherwise, `NSOKButton`.

## Discussion

The receiver’s values are recorded in `printInfo`.

## See Also

### Running the page setup dialog

func beginSheet(using: NSPrintInfo, on: NSWindow, completionHandler: ((NSPageLayout.Result) -> Void)?)

func beginSheet(with: NSPrintInfo, modalFor: NSWindow, delegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer?)

Presents a page setup sheet for the specified print info object, document-modal relative to the specified window.

Deprecated

func runModal() -> Int

Displays the page layout panel and begins the modal loop using the shared print info object.


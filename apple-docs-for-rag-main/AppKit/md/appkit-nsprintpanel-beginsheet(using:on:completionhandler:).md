

- AppKit
- NSPrintPanel
-  beginSheet(using:on:completionHandler:) 

Instance Method

# beginSheet(using:on:completionHandler:)

macOS 14.0+

``` source
@MainActor
func beginSheet(
    using printInfo: NSPrintInfo,
    on parentWindow: NSWindow,
    completionHandler handler: ((NSPrintPanel.Result) -> Void)? = nil
)
```

``` source
@MainActor
func beginSheet(
    using printInfo: NSPrintInfo,
    on parentWindow: NSWindow
) async -> NSPrintPanel.Result
```

## Discussion

## See Also

### Running the Panel

func beginSheet(with: NSPrintInfo, modalFor: NSWindow, delegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer?)

Displays a Print panel sheet and runs it modally for the specified window.

Deprecated

func runModal() -> Int

Displays the Print panel and begins the modal loop.

func runModal(with: NSPrintInfo) -> Int

Displays the Print panel and runs the modal loop using the specified printing information.


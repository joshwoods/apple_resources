

- AppKit
- NSPageLayout
-  beginSheet(using:on:completionHandler:) 

Instance Method

# beginSheet(using:on:completionHandler:)

macOS 14.0+

``` source
@MainActor
func beginSheet(
    using printInfo: NSPrintInfo,
    on parentWindow: NSWindow,
    completionHandler handler: ((NSPageLayout.Result) -> Void)? = nil
)
```

``` source
@MainActor
func beginSheet(
    using printInfo: NSPrintInfo,
    on parentWindow: NSWindow
) async -> NSPageLayout.Result
```

## See Also

### Running the page setup dialog

func beginSheet(with: NSPrintInfo, modalFor: NSWindow, delegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer?)

Presents a page setup sheet for the specified print info object, document-modal relative to the specified window.

Deprecated

func runModal() -> Int

Displays the page layout panel and begins the modal loop using the shared print info object.

func runModal(with: NSPrintInfo) -> Int

Displays the page layout panel and begins the modal loop using the specified print info object.


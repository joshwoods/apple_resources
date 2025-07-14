

- AppKit
- NSPageLayout
-  beginSheet(with:modalFor:delegate:didEnd:contextInfo:) Deprecated

Instance Method

# beginSheet(with:modalFor:delegate:didEnd:contextInfo:)

Presents a page setup sheet for the specified print info object, document-modal relative to the specified window.

macOS 10.0–15.4Deprecated

``` source
@MainActor
func beginSheet(
    with printInfo: NSPrintInfo,
    modalFor docWindow: NSWindow,
    delegate: Any?,
    didEnd didEndSelector: Selector?,
    contextInfo: UnsafeMutableRawPointer?
)
```

## Parameters 

`printInfo`  

The `NSPrintInfo` object to use.

`docWindow`  

The window to which the sheet is attached.

`delegate`  

The delegate to which `didEndSelector` is sent. Can be `nil`.

`didEndSelector`  

The selector sent to the delegate. Can be `nil`.

`contextInfo`  

Context information object passed with `didEndSelector`.

## Discussion

The `didEndSelector` argument must have the same signature as:

```
- (void)pageLayoutDidEnd:(NSPageLayout *)pageLayout returnCode:(int)returnCode  contextInfo: (void *)contextInfo;
```

The value passed as `returnCode` is either `NSCancelButton` or `NSOKButton`.

## See Also

### Running the page setup dialog

func beginSheet(using: NSPrintInfo, on: NSWindow, completionHandler: ((NSPageLayout.Result) -> Void)?)

func runModal() -> Int

Displays the page layout panel and begins the modal loop using the shared print info object.

func runModal(with: NSPrintInfo) -> Int

Displays the page layout panel and begins the modal loop using the specified print info object.


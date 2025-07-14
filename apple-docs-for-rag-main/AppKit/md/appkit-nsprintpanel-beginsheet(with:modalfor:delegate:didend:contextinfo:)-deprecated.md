

- AppKit
- NSPrintPanel
-  beginSheet(with:modalFor:delegate:didEnd:contextInfo:) Deprecated

Instance Method

# beginSheet(with:modalFor:delegate:didEnd:contextInfo:)

Displays a Print panel sheet and runs it modally for the specified window.

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

The printing information for the current job.

`docWindow`  

The window on which to display the sheet.

`delegate`  

A modal delegate object assigned to handle the closing of the Print panel sheet.

`didEndSelector`  

The selector to call on the modal delegate object when the sheet is dismissed. The signature of this method is listed in the Discussion section.

`contextInfo`  

A pointer to context data the `didEndSelector` method needs to process the sheet. This data is user-defined and may be `NULL`.

## Discussion

When the modal session ends, if `modalDelegate` and `didEndSelector` contain non-`nil` values, the method specified by `didEndSelector` is invoked on the object in `modalDelegate`. The data you specify in `contextInfo` is passed as a parameter to the `didEndSelector` method. The object in `modalDelegate` is not the same as a delegate assigned to the panel. Modal delegates for sheets are temporary and the relationship lasts only until the sheet is dismissed.

The `didEndSelector` argument must have the following signature:

```
- (void)printPanelDidEnd:(NSPrintPanel *)printPanel returnCode:(NSInteger)returnCode  contextInfo: (void *)contextInfo;
```

The value passed as `returnCode` is either `NSCancelButton` or `NSOKButton`. The value `NSOKButton` is returned even if the user clicked the Preview button.

## See Also

### Running the Panel

func beginSheet(using: NSPrintInfo, on: NSWindow, completionHandler: ((NSPrintPanel.Result) -> Void)?)

func runModal() -> Int

Displays the Print panel and begins the modal loop.

func runModal(with: NSPrintInfo) -> Int

Displays the Print panel and runs the modal loop using the specified printing information.


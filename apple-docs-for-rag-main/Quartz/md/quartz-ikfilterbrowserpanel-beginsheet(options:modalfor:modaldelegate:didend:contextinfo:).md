

- Quartz
- IKFilterBrowserPanel
-  beginSheet(options:modalFor:modalDelegate:didEnd:contextInfo:) 

Instance Method

# beginSheet(options:modalFor:modalDelegate:didEnd:contextInfo:)

Displays the filter browser in a sheet—that is, a dialog that is attached to its parent window and must be dismissed by the user.

macOS 10.4+

``` source
@MainActor
func beginSheet(
    options inOptions: [AnyHashable : Any]! = [:],
    modalFor docWindow: NSWindow!,
    modalDelegate: Any!,
    didEnd didEndSelector: Selector!,
    contextInfo: UnsafeMutableRawPointer!
)
```

## Parameters 

`inOptions`  

A dictionary of options that describe the configuration to use for the filter browser user interface. For the possible keys you can supply see Filter Browser Option Keys and the constant IKUISizeFlavor.

`docWindow`  

The parent window for the dialog.

`modalDelegate`  

The object that will invoke the selector `didEndSelector` when the filter browser session terminates.

`didEndSelector`  

The selector to invoke when the filter browser session terminates.

`contextInfo`  

Any data that must be passed as an argument to the delegate through `didEndSelector` after the filter browser session terminates.

## Discussion

When the filter browser session ends, `didEndSelector` is invoked on the modeless delegate, passing `contextInfo` as an argument. The selector `didEndSelector` must have the following signature:

`- (void)openPanelDidEnd:(NSOpenPanel *)panel returnCode:(int)returnCode contextInfo:(void *)contextInfo`

The `returnCode` value passed to the selector is set to NSOKButton if the user validates, or to NSCancelButton if the user cancels.

## See Also

### Displaying and Running the Panel

func filterBrowserView(options: [AnyHashable : Any]!) -> IKFilterBrowserView!

Returns a view that contains a filter browser.

func begin(options: [AnyHashable : Any]!, modelessDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Displays the filter browser in a new utility window, unless the filter browser is already open.

func runModal(options: [AnyHashable : Any]!) -> Int32

Displays the filter browser in a modal dialog that must be dismissed by the user but that is not attached to a window.

func finish(Any!)

Closes a filter browser view.




- Quartz
- IKFilterBrowserPanel
-  runModal(options:) 

Instance Method

# runModal(options:)

Displays the filter browser in a modal dialog that must be dismissed by the user but that is not attached to a window.

macOS 10.4+

``` source
@MainActor
func runModal(options inOptions: [AnyHashable : Any]! = [:]) -> Int32
```

## Parameters 

`inOptions`  

A dictionary of options that describe the configuration to use for the filter browser user interface. For the possible keys you can supply see Filter Browser Option Keys and the constant IKUISizeFlavor.

## Return Value

Either NSOKButton if the user validates, or NSCancelButton if the user cancels.

## See Also

### Displaying and Running the Panel

func filterBrowserView(options: [AnyHashable : Any]!) -> IKFilterBrowserView!

Returns a view that contains a filter browser.

func begin(options: [AnyHashable : Any]!, modelessDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Displays the filter browser in a new utility window, unless the filter browser is already open.

func beginSheet(options: [AnyHashable : Any]!, modalFor: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Displays the filter browser in a sheet—that is, a dialog that is attached to its parent window and must be dismissed by the user.

func finish(Any!)

Closes a filter browser view.


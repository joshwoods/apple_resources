

- Quartz
- IKFilterBrowserPanel
-  finish(\_:) 

Instance Method

# finish(\_:)

Closes a filter browser view.

macOS 10.4+

``` source
@MainActor
func finish(_ sender: Any!)
```

## Parameters 

`sender`  

The object that invokes the action, such as an OK or Cancel button.

## Discussion

Invoke this action when you want to dismiss the filter browser.

## See Also

### Displaying and Running the Panel

func filterBrowserView(options: [AnyHashable : Any]!) -> IKFilterBrowserView!

Returns a view that contains a filter browser.

func begin(options: [AnyHashable : Any]!, modelessDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Displays the filter browser in a new utility window, unless the filter browser is already open.

func beginSheet(options: [AnyHashable : Any]!, modalFor: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Displays the filter browser in a sheet—that is, a dialog that is attached to its parent window and must be dismissed by the user.

func runModal(options: [AnyHashable : Any]!) -> Int32

Displays the filter browser in a modal dialog that must be dismissed by the user but that is not attached to a window.




- WebKit
- WKWebExtension
- WKWebExtension.Action
-  popupPopover 

Instance Property

# popupPopover

A popover that presents a web view loaded with the pop-up page for this action, or `nil` if no popup is specified.

macOS 15.4+

``` source
@MainActor
var popupPopover: NSPopover? { get }
```

## Discussion

This popover contains a view controller with a web view preloaded with the pop-up page. It automatically adjusts its size to fit the web view’s content size. The presentsPopup property should be checked to determine the availability of a pop-up before using this property. Dismissing the popover will close the pop-up and unload the web view.

## See Also

### Related Documentation

var presentsPopup: Bool

A Boolean value indicating whether the action has a pop-up.


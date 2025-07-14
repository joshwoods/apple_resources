

- WebKit
- WKWebExtension
- WKWebExtension.Action
-  popupWebView 

Instance Property

# popupWebView

A web view loaded with the pop-up page for this action, or `nil` if no pop-up is specified.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var popupWebView: WKWebView? { get }
```

## Discussion

The web view will be preloaded with the pop-up page upon first access or after it has been unloaded. Use the presentsPopup property to determine whether a pop-up should be displayed before using this property.

## See Also

### Related Documentation

var presentsPopup: Bool

A Boolean value indicating whether the action has a pop-up.


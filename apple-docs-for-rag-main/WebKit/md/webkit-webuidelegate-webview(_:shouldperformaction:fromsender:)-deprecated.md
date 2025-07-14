

- WebKit
- WebUIDelegate
-  webView(\_:shouldPerformAction:fromSender:) Deprecated

Instance Method

# webView(\_:shouldPerformAction:fromSender:)

Returns a Boolean value that indicates whether the action sent by the specified object should be performed.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    shouldPerformAction action: Selector!,
    fromSender sender: Any!
) -> Bool
```

## Parameters 

`webView`  

The web view that sent the message.

`action`  

The action to perform. See WebView for information on actions a web view can perform.

`sender`  

The object that sent the action.

## Return Value

true if the action should be performed; otherwise, false.

## Discussion

This method allows the delegate to control the web view’s behavior when action methods are invoked. For example, if the action is `copy:`, the delegate can return false to perform a copy in some other way than the default.

## See Also

### Controlling Other Behaviors

func webView(WebView!, validate: (any NSValidatedUserInterfaceItem)!, defaultValidation: Bool) -> Bool

Returns a Boolean value that indicates whether the specified user interface item is valid.

Deprecated


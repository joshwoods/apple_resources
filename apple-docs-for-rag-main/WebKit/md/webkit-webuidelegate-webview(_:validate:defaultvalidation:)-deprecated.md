

- WebKit
- WebUIDelegate
-  webView(\_:validate:defaultValidation:) Deprecated

Instance Method

# webView(\_:validate:defaultValidation:)

Returns a Boolean value that indicates whether the specified user interface item is valid.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    validate item: (any NSValidatedUserInterfaceItem)!,
    defaultValidation: Bool
) -> Bool
```

## Parameters 

`webView`  

The web view that sent the message.

`item`  

The user interface item being validated.

`defaultValidation`  

true if the web view believes the user interface item is valid; otherwise, false.

## Return Value

true if the specified user interface item is valid; otherwise, false.

## Discussion

See NSUserInterfaceValidations and NSValidatedUserInterfaceItem for more information about user interface validation. If you do not implement this method, the value of `defaultValidation` is used.

## See Also

### Controlling Other Behaviors

func webView(WebView!, shouldPerformAction: Selector!, fromSender: Any!) -> Bool

Returns a Boolean value that indicates whether the action sent by the specified object should be performed.

Deprecated


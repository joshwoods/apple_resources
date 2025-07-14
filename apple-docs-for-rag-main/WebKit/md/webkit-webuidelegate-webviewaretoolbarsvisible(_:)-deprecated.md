

- WebKit
- WebUIDelegate
-  webViewAreToolbarsVisible(\_:) Deprecated

Instance Method

# webViewAreToolbarsVisible(\_:)

Returns a Boolean value indicating whether any toolbars are visible in a web view’s window.

macOS 10.3–10.14Deprecated

``` source
optional func webViewAreToolbarsVisible(_ sender: WebView!) -> Bool
```

## Parameters 

`sender`  

The web view that sent the message.

## Return Value

true if a web view’s window has any toolbars that are currently visible (other than the status bar); otherwise, false.

## See Also

### Managing Toolbars and the Status Bar

func webView(WebView!, setToolbarsVisible: Bool)

Sets whether a web view’s toolbars should be visible.

Deprecated

func webViewIsStatusBarVisible(WebView!) -> Bool

Returns a Boolean value indicating whether the status bar in a web view’s window is visible.

Deprecated

func webView(WebView!, setStatusBarVisible: Bool)

Sets the visibility of the status bar in a web view’s window.

Deprecated


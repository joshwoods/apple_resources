

- WebKit
- WebUIDelegate
-  webView(\_:setStatusBarVisible:) Deprecated

Instance Method

# webView(\_:setStatusBarVisible:)

Sets the visibility of the status bar in a web view’s window.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    setStatusBarVisible visible: Bool
)
```

## Parameters 

`sender`  

The web view that sent the message.

`visible`  

If true, the delegate should display the status bar (if any); if false, the delegate should hide the status bar.

## Discussion

No action is taken if you do not implement this method.

## See Also

### Managing Toolbars and the Status Bar

func webViewAreToolbarsVisible(WebView!) -> Bool

Returns a Boolean value indicating whether any toolbars are visible in a web view’s window.

Deprecated

func webView(WebView!, setToolbarsVisible: Bool)

Sets whether a web view’s toolbars should be visible.

Deprecated

func webViewIsStatusBarVisible(WebView!) -> Bool

Returns a Boolean value indicating whether the status bar in a web view’s window is visible.

Deprecated


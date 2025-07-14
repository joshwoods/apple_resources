

- WebKit
- WebUIDelegate
-  webView(\_:setToolbarsVisible:) Deprecated

Instance Method

# webView(\_:setToolbarsVisible:)

Sets whether a web view’s toolbars should be visible.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    setToolbarsVisible visible: Bool
)
```

## Parameters 

`sender`  

The web view that sent the message.

`visible`  

If true, all toolbars (with the exception of the status bar) are shown; otherwise, all toolbars (with the exception of the status bar) are removed.

## Discussion

No action is taken if you do not implement this method.

## See Also

### Managing Toolbars and the Status Bar

func webViewAreToolbarsVisible(WebView!) -> Bool

Returns a Boolean value indicating whether any toolbars are visible in a web view’s window.

Deprecated

func webViewIsStatusBarVisible(WebView!) -> Bool

Returns a Boolean value indicating whether the status bar in a web view’s window is visible.

Deprecated

func webView(WebView!, setStatusBarVisible: Bool)

Sets the visibility of the status bar in a web view’s window.

Deprecated


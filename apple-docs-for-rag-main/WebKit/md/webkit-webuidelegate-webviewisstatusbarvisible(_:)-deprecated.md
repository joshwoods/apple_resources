

- WebKit
- WebUIDelegate
-  webViewIsStatusBarVisible(\_:) Deprecated

Instance Method

# webViewIsStatusBarVisible(\_:)

Returns a Boolean value indicating whether the status bar in a web view’s window is visible.

macOS 10.3–10.14Deprecated

``` source
optional func webViewIsStatusBarVisible(_ sender: WebView!) -> Bool
```

## Parameters 

`sender`  

The web view that sent the message.

## Return Value

true if a web view’s status bar (if any) is visible; otherwise, false.

## Discussion

If you do not implement this method, it returns false by default.

## See Also

### Managing Toolbars and the Status Bar

func webViewAreToolbarsVisible(WebView!) -> Bool

Returns a Boolean value indicating whether any toolbars are visible in a web view’s window.

Deprecated

func webView(WebView!, setToolbarsVisible: Bool)

Sets whether a web view’s toolbars should be visible.

Deprecated

func webView(WebView!, setStatusBarVisible: Bool)

Sets the visibility of the status bar in a web view’s window.

Deprecated


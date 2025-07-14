

- WebKit
- WKUIDelegate
-  webView(\_:willDismissEditMenuWithAnimator:) 

Instance Method

# webView(\_:willDismissEditMenuWithAnimator:)

Tells the delegate that the web view is about to dismiss an edit menu.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    willDismissEditMenuWithAnimator animator: any UIEditMenuInteractionAnimating
)
```

## See Also

### Displaying an edit menu

func webView(WKWebView, willPresentEditMenuWithAnimator: any UIEditMenuInteractionAnimating)

Tells the delegate that the web view is about to present an edit menu.


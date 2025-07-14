

- UIKit
- UIWebViewDelegate
-  webView(\_:didFailLoadWithError:) Deprecated

Instance Method

# webView(\_:didFailLoadWithError:)

Sent if a web view failed to load a frame.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0Deprecated

``` source
@MainActor
optional func webView(
    _ webView: UIWebView,
    didFailLoadWithError error: any Error
)
```

## Parameters 

`webView`  

The web view that failed to load a frame.

`error`  

The error that occurred during loading.

## See Also

### Loading Content

func webView(UIWebView, shouldStartLoadWith: URLRequest, navigationType: UIWebView.NavigationType) -> Bool

Sent before a web view begins loading a frame.

Deprecated

func webViewDidStartLoad(UIWebView)

Sent after a web view starts loading a frame.

Deprecated

func webViewDidFinishLoad(UIWebView)

Sent after a web view finishes loading a frame.

Deprecated


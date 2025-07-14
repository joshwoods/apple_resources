

- UIKit
- UIWebViewDelegate
-  webViewDidStartLoad(\_:) Deprecated

Instance Method

# webViewDidStartLoad(\_:)

Sent after a web view starts loading a frame.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0Deprecated

``` source
@MainActor
optional func webViewDidStartLoad(_ webView: UIWebView)
```

## Parameters 

`webView`  

The web view that has begun loading a new frame.

## See Also

### Loading Content

func webView(UIWebView, shouldStartLoadWith: URLRequest, navigationType: UIWebView.NavigationType) -> Bool

Sent before a web view begins loading a frame.

Deprecated

func webViewDidFinishLoad(UIWebView)

Sent after a web view finishes loading a frame.

Deprecated

func webView(UIWebView, didFailLoadWithError: any Error)

Sent if a web view failed to load a frame.

Deprecated


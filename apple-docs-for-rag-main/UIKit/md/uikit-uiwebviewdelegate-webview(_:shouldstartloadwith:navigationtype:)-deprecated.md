

- UIKit
- UIWebViewDelegate
-  webView(\_:shouldStartLoadWith:navigationType:) Deprecated

Instance Method

# webView(\_:shouldStartLoadWith:navigationType:)

Sent before a web view begins loading a frame.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0Deprecated

``` source
@MainActor
optional func webView(
    _ webView: UIWebView,
    shouldStartLoadWith request: URLRequest,
    navigationType: UIWebView.NavigationType
) -> Bool
```

## Parameters 

`webView`  

The web view that is about to load a new frame.

`request`  

The content location.

`navigationType`  

The type of user action that started the load request.

## Return Value

true if the web view should begin loading content; otherwise, false .

## See Also

### Loading Content

func webViewDidStartLoad(UIWebView)

Sent after a web view starts loading a frame.

Deprecated

func webViewDidFinishLoad(UIWebView)

Sent after a web view finishes loading a frame.

Deprecated

func webView(UIWebView, didFailLoadWithError: any Error)

Sent if a web view failed to load a frame.

Deprecated


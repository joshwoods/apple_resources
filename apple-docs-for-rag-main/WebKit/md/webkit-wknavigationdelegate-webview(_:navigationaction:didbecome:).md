

- WebKit
- WKNavigationDelegate
-  webView(\_:navigationAction:didBecome:) 

Instance Method

# webView(\_:navigationAction:didBecome:)

Tells the delegate that a navigation action became a download.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    navigationAction: WKNavigationAction,
    didBecome download: WKDownload
)
```

## Parameters 

`webView`  

The web view in which the navigation action took place.

`navigationAction`  

Descriptive information about the navigation response that turned into a download.

`download`  

An object that represents the download of a web resource.

## Discussion

Implement this method to begin tracking download progress.

## See Also

### Handling download progress

func webView(WKWebView, navigationResponse: WKNavigationResponse, didBecome: WKDownload)

Tells the delegate that a navigation response became a download.


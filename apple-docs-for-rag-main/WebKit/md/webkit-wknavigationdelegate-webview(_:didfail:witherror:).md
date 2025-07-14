

- WebKit
- WKNavigationDelegate
-  webView(\_:didFail:withError:) 

Instance Method

# webView(\_:didFail:withError:)

Tells the delegate that an error occurred during navigation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    didFail navigation: WKNavigation!,
    withError error: any Error
)
```

## Parameters 

`webView`  

The web view that reported the error.

`navigation`  

The navigation object for the operation. This object corresponds to a WKNavigation object that WebKit returned when the load operation began. You use it to track the progress of that operation.

`error`  

The error that occurred.

## Mentioned in 

Replacing UIWebView in your app

## See Also

### Responding to navigation errors

func webView(WKWebView, didFailProvisionalNavigation: WKNavigation!, withError: any Error)

Tells the delegate that an error occurred during the early navigation process.

func webViewWebContentProcessDidTerminate(WKWebView)

Tells the delegate that the web view’s content process was terminated.




- WebKit
- WKNavigationDelegate
-  webViewWebContentProcessDidTerminate(\_:) 

Instance Method

# webViewWebContentProcessDidTerminate(\_:)

Tells the delegate that the web view’s content process was terminated.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
@MainActor
optional func webViewWebContentProcessDidTerminate(_ webView: WKWebView)
```

## Parameters 

`webView`  

The web view whose underlying web content process was terminated.

## Discussion

Web views use a separate process to render and manage web content. WebKit calls this method when the process for the specified web view terminates for any reason.

## See Also

### Responding to navigation errors

func webView(WKWebView, didFail: WKNavigation!, withError: any Error)

Tells the delegate that an error occurred during navigation.

func webView(WKWebView, didFailProvisionalNavigation: WKNavigation!, withError: any Error)

Tells the delegate that an error occurred during the early navigation process.


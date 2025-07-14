

- WebKit
-  Replacing UIWebView in your app 

Article

# Replacing UIWebView in your app

Find a suitable alternative to handle your app’s web content.

## Overview

If your app is using UIWebView, you need to replace it with another Apple technology, because this class is now deprecated. Choose among several technologies, based on your app’s functionality and the degree of configurability you need. This article explores some alternatives and specifically the configuration and architectural changes of WKWebView.

### Consider alternative technologies

Before beginning a migration away from UIWebView, consider whether it can be replaced with other tools. Apple has a variety of technologies that can replace a web view to accomplish similar functionality, and possibly a richer feature set with less code.

If you need an in-app web browser and don’t need deep customization of that experience, SFSafariViewController is a good choice. It handles all the features you’d need to implement in a basic browser and more.

If you need to authenticate your users, use ASWebAuthenticationSession.

If you need to display maps or map tiles, consider using MKMapView.

### Update to WKWebView

If you need a high degree of configurability or are using web content in ways unrelated to browsing, use WKWebView.

WKWebView isn’t a drop-in replacement for UIWebView. It has a different architecture that requires rethinking how you use web views, as well as code changes to implement its functionality. You may not be able to implement some features in WKWebView.

### Implement delegates for functionality

WKWebView uses various delegates to implement functionality that’s similar to UIWebViewDelegate. The table below shows the UIWebViewDelegate methods and their WKWebView equivalents in the WKNavigationDelegate column.

| `UIWebViewDelegate` | `WKNavigationDelegate` |
|----|----|
| webViewDidStartLoad(_:) | webView(_:didStartProvisionalNavigation:) |
| webViewDidFinishLoad(_:) | webView(_:didFinish:) |
| webView(_:didFailLoadWithError:) | webView(_:didFailProvisionalNavigation:withError:) or webView(_:didFail:withError:) |
| webView(_:shouldStartLoadWith:navigationType:) | webView(_:decidePolicyFor:decisionHandler:) or webView(_:decidePolicyFor:decisionHandler:) |
| connection(_:didReceive:) | webView(_:didReceive:completionHandler:) |

Note

The webView(_:decidePolicyFor:decisionHandler:) function doesn’t return a Boolean as its UIWebView counterpart did; it uses the `decisionHandler` to return an WKNavigationActionPolicy.allow or WKNavigationActionPolicy.cancel value.

### Plan for architectural changes

One major architectural difference between UIWebView and WKWebView is that the methods of WKWebView tend to be asynchronous, while the methods of UIWebView were synchronous.

This difference requires code and architecture changes in your app. Another major change relates to creating single sign on (SSO) functionality. Cookie restrictions across the entire WKWebView landscape, mean SSO functionality in WKWebView isn’t supported for third-party cookies and clients should use a token-based authentication system like OAuth for SSO. Third-party cookies are cookies for a domain other than the domain for which the context was loaded. APIs in the Authentication Services framework are specifically built to do this.

## See Also

### Web view

Viewing Desktop or Mobile Web Content Using a Web View

Implement a simple iPad web browser that can view either the desktop or mobile version of a website.

class WKWebView

An object that displays interactive web content, such as for an in-app browser.

protocol WKUIDelegate

The methods for presenting native user interface elements on behalf of a webpage.




- WebKit
-  WebPolicyDelegate Deprecated

Protocol

# WebPolicyDelegate

macOS 10.3–10.14Deprecated

``` source
protocol WebPolicyDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func webView(WebView!, decidePolicyForMIMEType: String!, request: URLRequest!, frame: WebFrame!, decisionListener: (any WebPolicyDecisionListener)!)

Decides whether to display content with a given MIME type.

func webView(WebView!, decidePolicyForNavigationAction: [AnyHashable : Any]!, request: URLRequest!, frame: WebFrame!, decisionListener: (any WebPolicyDecisionListener)!)

Routes a navigation action internally or to an external viewer.

func webView(WebView!, decidePolicyForNewWindowAction: [AnyHashable : Any]!, request: URLRequest!, newFrameName: String!, decisionListener: (any WebPolicyDecisionListener)!)

Decides whether to allow a targeted navigation event, such as opening a link in a new window.

func webView(WebView!, unableToImplementPolicyWithError: (any Error)!, frame: WebFrame!)

Handles or drops events that were rejected by a policy maker.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Related Documentation

WebKit Objective-C Programming Guide

### Setting Policies (Legacy)

protocol WebPolicyDecisionListener

This protocol enables WebView policy delegates to communicate with listener objects. A listener object conforming to this protocol is passed as one of the arguments to web view policy delegate methods.

Deprecated




- WebKit
-  WKNavigationDelegate 

Protocol

# WKNavigationDelegate

Methods for accepting or rejecting navigation changes, and for tracking the progress of navigation requests.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
@MainActor
protocol WKNavigationDelegate : NSObjectProtocol
```

## Mentioned in 

Replacing UIWebView in your app

## Overview

Implement the methods of the WKNavigationDelegate protocol in the object you use to coordinate changes in your web view’s main frame. As the user attempts to navigate web content, the web view coordinates with its navigation delegate to manage any transitions. For example, you might use these methods to restrict navigation from specific links within your content. You might also use them to track the progress of requests, and to respond to errors and authentication challenges.

## Topics

### Allowing or denying navigation requests

func webView(WKWebView, decidePolicyFor: WKNavigationAction, preferences: WKWebpagePreferences, decisionHandler: (WKNavigationActionPolicy, WKWebpagePreferences) -> Void)

Asks the delegate for permission to navigate to new content based on the specified preferences and action information.

func webView(WKWebView, decidePolicyFor: WKNavigationAction, decisionHandler: (WKNavigationActionPolicy) -> Void)

Asks the delegate for permission to navigate to new content based on the specified action information.

enum WKNavigationActionPolicy

Constants that indicate whether to allow or cancel navigation to a webpage from an action.

func webView(WKWebView, decidePolicyFor: WKNavigationResponse, decisionHandler: (WKNavigationResponsePolicy) -> Void)

Asks the delegate for permission to navigate to new content after the response to the navigation request is known.

enum WKNavigationResponsePolicy

Constants that indicate whether to allow or cancel navigation to a webpage from a response.

### Tracking the load progress of a request

func webView(WKWebView, didStartProvisionalNavigation: WKNavigation!)

Tells the delegate that navigation from the main frame has started.

func webView(WKWebView, didReceiveServerRedirectForProvisionalNavigation: WKNavigation!)

Tells the delegate that the web view received a server redirect for a request.

func webView(WKWebView, didCommit: WKNavigation!)

Tells the delegate that the web view has started to receive content for the main frame.

func webView(WKWebView, didFinish: WKNavigation!)

Tells the delegate that navigation is complete.

### Responding to authentication challenges

func webView(WKWebView, didReceive: URLAuthenticationChallenge, completionHandler: (URLSession.AuthChallengeDisposition, URLCredential?) -> Void)

Asks the delegate to respond to an authentication challenge.

func webView(WKWebView, authenticationChallenge: URLAuthenticationChallenge, shouldAllowDeprecatedTLS: (Bool) -> Void)

Asks the delegate whether to continue with a connection that uses a deprecated version of TLS.

### Responding to navigation errors

func webView(WKWebView, didFail: WKNavigation!, withError: any Error)

Tells the delegate that an error occurred during navigation.

func webView(WKWebView, didFailProvisionalNavigation: WKNavigation!, withError: any Error)

Tells the delegate that an error occurred during the early navigation process.

func webViewWebContentProcessDidTerminate(WKWebView)

Tells the delegate that the web view’s content process was terminated.

### Handling download progress

func webView(WKWebView, navigationResponse: WKNavigationResponse, didBecome: WKDownload)

Tells the delegate that a navigation response became a download.

func webView(WKWebView, navigationAction: WKNavigationAction, didBecome: WKDownload)

Tells the delegate that a navigation action became a download.

### Instance Methods

func webView(WKWebView, shouldGoTo: WKBackForwardListItem, willUseInstantBack: Bool, completionHandler: (Bool) -> Void)

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Navigation

class WKBackForwardList

An object that manages the list of previously loaded webpages, which the web view uses for forward and backward navigation.

class WKBackForwardListItem

A representation of a webpage that the web view previously visited.

class WKNavigation

An object that tracks the loading progress of a webpage.

class WKNavigationAction

An object that contains information about an action that causes navigation to occur.

class WKNavigationResponse

An object that contains the response to a navigation request, and which you use to make navigation-related policy decisions.




- WebKit
-  WKNavigationActionPolicy 

Enumeration

# WKNavigationActionPolicy

Constants that indicate whether to allow or cancel navigation to a webpage from an action.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
enum WKNavigationActionPolicy
```

## Topics

### Constants

case cancel

Cancel the navigation.

case allow

Allow the navigation to continue.

case download

Allow the download to proceed.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Allowing or denying navigation requests

func webView(WKWebView, decidePolicyFor: WKNavigationAction, preferences: WKWebpagePreferences, decisionHandler: (WKNavigationActionPolicy, WKWebpagePreferences) -> Void)

Asks the delegate for permission to navigate to new content based on the specified preferences and action information.

func webView(WKWebView, decidePolicyFor: WKNavigationAction, decisionHandler: (WKNavigationActionPolicy) -> Void)

Asks the delegate for permission to navigate to new content based on the specified action information.

func webView(WKWebView, decidePolicyFor: WKNavigationResponse, decisionHandler: (WKNavigationResponsePolicy) -> Void)

Asks the delegate for permission to navigate to new content after the response to the navigation request is known.

enum WKNavigationResponsePolicy

Constants that indicate whether to allow or cancel navigation to a webpage from a response.


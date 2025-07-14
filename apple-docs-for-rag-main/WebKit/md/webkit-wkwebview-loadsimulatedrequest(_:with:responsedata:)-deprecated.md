

- WebKit
- WKWebView
-  loadSimulatedRequest(\_:with:responseData:) Deprecated

Instance Method

# loadSimulatedRequest(\_:with:responseData:)

iOS 15.0–15.0DeprecatediPadOS 15.0–15.0DeprecatedMac Catalyst 15.0–15.0DeprecatedmacOS 12.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func loadSimulatedRequest(
    _ request: URLRequest,
    with response: URLResponse,
    responseData data: Data
) -> WKNavigation
```

Deprecated

Use loadSimulatedRequest(_:response:responseData:) instead.

## See Also

### Deprecated

var certificateChain: [Any]

An array of objects forming the certificate chain for the currently committed navigation.

Deprecated

func closeAllMediaPresentations()Deprecated

func loadSimulatedRequest(URLRequest, withResponseHTML: String) -> WKNavigationDeprecated


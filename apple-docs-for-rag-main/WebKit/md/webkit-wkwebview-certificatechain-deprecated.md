

- WebKit
- WKWebView
-  certificateChain Deprecated

Instance Property

# certificateChain

An array of objects forming the certificate chain for the currently committed navigation.

iOS 9.0–10.0DeprecatediPadOS 9.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.11–10.12DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var certificateChain: [Any] { get }
```

Deprecated

Use serverTrust instead.

## Discussion

Each item in the array is a SecCertificate object.

## See Also

### Deprecated

func closeAllMediaPresentations()Deprecated

func loadSimulatedRequest(URLRequest, with: URLResponse, responseData: Data) -> WKNavigationDeprecated

func loadSimulatedRequest(URLRequest, withResponseHTML: String) -> WKNavigationDeprecated


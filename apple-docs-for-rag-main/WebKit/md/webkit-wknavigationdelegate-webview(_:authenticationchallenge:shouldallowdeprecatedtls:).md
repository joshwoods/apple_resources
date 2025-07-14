

- WebKit
- WKNavigationDelegate
-  webView(\_:authenticationChallenge:shouldAllowDeprecatedTLS:) 

Instance Method

# webView(\_:authenticationChallenge:shouldAllowDeprecatedTLS:)

Asks the delegate whether to continue with a connection that uses a deprecated version of TLS.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    authenticationChallenge challenge: URLAuthenticationChallenge,
    shouldAllowDeprecatedTLS decisionHandler: @escaping @MainActor (Bool) -> Void
)
```

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    shouldAllowDeprecatedTLSFor challenge: URLAuthenticationChallenge
) async -> Bool
```

## Parameters 

`webView`  

The web view that receives the authentication challenge.

`challenge`  

The authentication challenge.

`decisionHandler`  

The completion handler block to execute with the decision. This handler has no return value and takes the following parameter:

decision  
A Boolean value that indicates whether to continue to use a deprecated version of TLS. Specify true to continue, or false to reject the connection.

## Discussion

If you don’t implement this method, the web view uses system settings to determine whether to allow the use of deprecated versions of TLS.

## See Also

### Responding to authentication challenges

func webView(WKWebView, didReceive: URLAuthenticationChallenge, completionHandler: (URLSession.AuthChallengeDisposition, URLCredential?) -> Void)

Asks the delegate to respond to an authentication challenge.


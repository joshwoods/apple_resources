

- WebKit
- WKNavigationDelegate
-  webView(\_:didReceive:completionHandler:) 

Instance Method

# webView(\_:didReceive:completionHandler:)

Asks the delegate to respond to an authentication challenge.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    didReceive challenge: URLAuthenticationChallenge,
    completionHandler: @escaping @MainActor (URLSession.AuthChallengeDisposition, URLCredential?) -> Void
)
```

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    respondTo challenge: URLAuthenticationChallenge
) async -> (URLSession.AuthChallengeDisposition, URLCredential?)
```

## Parameters 

`webView`  

The web view that receives the authentication challenge.

`challenge`  

The authentication challenge.

`completionHandler`  

A completion handler block to execute with the response. This handler has no return value and takes the following parameters:

disposition  
The option to use to handle the challenge. For a list of options, see URLSession.AuthChallengeDisposition.

credential  
The credential to use for authentication when the `disposition` parameter contains the value URLSession.AuthChallengeDisposition.useCredential. Specify `nil` to continue without a credential.

## Mentioned in 

Replacing UIWebView in your app

## Discussion

If you don’t implement this method, the web view responds to the authentication challenge with the URLSession.AuthChallengeDisposition.rejectProtectionSpace disposition.

## See Also

### Responding to authentication challenges

func webView(WKWebView, authenticationChallenge: URLAuthenticationChallenge, shouldAllowDeprecatedTLS: (Bool) -> Void)

Asks the delegate whether to continue with a connection that uses a deprecated version of TLS.


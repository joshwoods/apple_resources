

- Authentication Services
- ASWebAuthenticationSessionWebBrowserSessionManager
-  shared 

Type Property

# shared

The shared manager for which a web browser acts as the session handler.

macOS 10.15+

``` source
class var shared: ASWebAuthenticationSessionWebBrowserSessionManager { get }
```

## Discussion

Use this singleton when supporting single sign-on (SSO) in a web browser app. Make the web browser adopt the ASWebAuthenticationSessionWebBrowserSessionHandling protocol, and set it as the shared manager’s sessionHandler. This allows your browser app to receive and process ASWebAuthenticationSessionRequest instances from other apps.


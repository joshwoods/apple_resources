

- Authentication Services
- ASWebAuthenticationSessionWebBrowserSessionManager
-  sessionHandler 

Instance Property

# sessionHandler

A handler that a web browser provides to handle session requests from an app.

macOS 10.15+

``` source
var sessionHandler: any ASWebAuthenticationSessionWebBrowserSessionHandling { get set }
```

## Mentioned in 

Supporting Single Sign-On in a Web Browser App

## Discussion

To enable a web browser that you write to participate in single sign-on (SSO), adopt the ASWebAuthenticationSessionWebBrowserSessionHandling protocol, and then set your browser app as the shared manager’s sessionHandler.

## See Also

### Handling a Session Request

protocol ASWebAuthenticationSessionWebBrowserSessionHandling

An interface that a session handler implements to handle login requests from an app.




- Authentication Services
- ASWebAuthenticationSessionRequest
-  url 

Instance Property

# url

The web address the browser should use to perform the authentication request.

macOS 10.15+

``` source
var url: URL { get }
```

## Mentioned in 

Supporting Single Sign-On in a Web Browser App

## See Also

### Interpreting a Request

var callbackURLScheme: String?

The scheme the browser should use to return the result of the authentication attempt to the app requesting it.

Deprecated

var shouldUseEphemeralSession: Bool

A Boolean that indicates whether the browser should use a private browsing session.

var uuid: UUID

A unique identifier for the request.


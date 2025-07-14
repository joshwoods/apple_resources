

- Authentication Services
- ASWebAuthenticationSessionRequest
-  shouldUseEphemeralSession 

Instance Property

# shouldUseEphemeralSession

A Boolean that indicates whether the browser should use a private browsing session.

macOS 10.15+

``` source
var shouldUseEphemeralSession: Bool { get }
```

## Mentioned in 

Supporting Single Sign-On in a Web Browser App

## See Also

### Interpreting a Request

var url: URL

The web address the browser should use to perform the authentication request.

var callbackURLScheme: String?

The scheme the browser should use to return the result of the authentication attempt to the app requesting it.

Deprecated

var uuid: UUID

A unique identifier for the request.


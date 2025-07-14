

- Authentication Services
- ASWebAuthenticationSessionRequest
-  callbackURLScheme Deprecated

Instance Property

# callbackURLScheme

The scheme the browser should use to return the result of the authentication attempt to the app requesting it.

macOS 10.15–14.4Deprecated

``` source
var callbackURLScheme: String? { get }
```

## Mentioned in 

Supporting Single Sign-On in a Web Browser App

## See Also

### Interpreting a Request

var url: URL

The web address the browser should use to perform the authentication request.

var shouldUseEphemeralSession: Bool

A Boolean that indicates whether the browser should use a private browsing session.

var uuid: UUID

A unique identifier for the request.


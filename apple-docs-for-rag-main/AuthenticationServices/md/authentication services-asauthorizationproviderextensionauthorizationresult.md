

- Authentication Services
-  ASAuthorizationProviderExtensionAuthorizationResult 

Class

# ASAuthorizationProviderExtensionAuthorizationResult

The result of an authorization request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
class ASAuthorizationProviderExtensionAuthorizationResult
```

## Topics

### Initializers

init(httpAuthorizationHeaders: [String : String])

Initializes an authorization with tokens stored in HTTP headers.

init(httpResponse: HTTPURLResponse, httpBody: Data?)

Initializes an authorization with a HTTP response and body.

### Instance Properties

var httpAuthorizationHeaders: [String : String]?

A dictionary of authorization HTTP headers.

var httpResponse: HTTPURLResponse?

The HTTP response for authentications.

var httpBody: Data?

The HTTP response body.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Performing enterprise single sign-on

class ASAuthorizationSingleSignOnProvider

A mechanism for generating requests to authenticate users with third-party providers.

class ASAuthorizationSingleSignOnCredential

A credential that results from a successful single sign-on (SSO) authentication.

protocol ASAuthorizationProviderExtensionAuthorizationRequestHandler

An interface through which a single sign-on (SSO) authentication provider extension handles authentication requests.

struct RequestOptions

Options that modify how a controller performs authorization requests.


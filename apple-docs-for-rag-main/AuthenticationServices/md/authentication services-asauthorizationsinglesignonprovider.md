

- Authentication Services
-  ASAuthorizationSingleSignOnProvider 

Class

# ASAuthorizationSingleSignOnProvider

A mechanism for generating requests to authenticate users with third-party providers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class ASAuthorizationSingleSignOnProvider
```

## Topics

### Creating an Authorization Provider

convenience init(identityProvider: URL)

Creates a single sign-on (SSO) authorization provider.

### Creating Authorization Requests

var canPerformAuthorization: Bool

A Boolean value that indicates if the provider is capable of performing authorization within a given configuration.

func createRequest() -> ASAuthorizationSingleSignOnRequest

Creates a single sign-on (SSO) authorization request.

class ASAuthorizationSingleSignOnRequest

An OpenID authorization request that provides single sign-on (SSO) functionality.

class ASAuthorizationOpenIDRequest

An OpenID authorization request.

### Identifying the Identity Provider

var url: URL

The URL of the identity provider.

## Relationships

### Inherits From

- NSObject

### Conforms To

- ASAuthorizationProvider
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Performing enterprise single sign-on

class ASAuthorizationSingleSignOnCredential

A credential that results from a successful single sign-on (SSO) authentication.

protocol ASAuthorizationProviderExtensionAuthorizationRequestHandler

An interface through which a single sign-on (SSO) authentication provider extension handles authentication requests.

class ASAuthorizationProviderExtensionAuthorizationResult

The result of an authorization request.

struct RequestOptions

Options that modify how a controller performs authorization requests.


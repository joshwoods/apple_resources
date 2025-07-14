

- Authentication Services
-  ASAuthorizationSingleSignOnCredential 

Class

# ASAuthorizationSingleSignOnCredential

A credential that results from a successful single sign-on (SSO) authentication.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class ASAuthorizationSingleSignOnCredential
```

## Topics

### Identifying a User

var identityToken: Data?

A JSON Web Token (JWT) that securely communicates information about the user to your app.

var accessToken: Data?

An access token used to get an identity token.

var state: String?

An arbitrary string that your app provided to the request that generated this credential.

var authorizedScopes: [ASAuthorization.Scope]

The contact information the user authorized your app to access.

### Parsing the Response

var authenticatedResponse: HTTPURLResponse?

The complete response authentication, including technology-specific values.

## Relationships

### Inherits From

- NSObject

### Conforms To

- ASAuthorizationCredential
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Performing enterprise single sign-on

class ASAuthorizationSingleSignOnProvider

A mechanism for generating requests to authenticate users with third-party providers.

protocol ASAuthorizationProviderExtensionAuthorizationRequestHandler

An interface through which a single sign-on (SSO) authentication provider extension handles authentication requests.

class ASAuthorizationProviderExtensionAuthorizationResult

The result of an authorization request.

struct RequestOptions

Options that modify how a controller performs authorization requests.


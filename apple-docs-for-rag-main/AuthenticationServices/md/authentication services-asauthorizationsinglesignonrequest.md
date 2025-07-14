

- Authentication Services
-  ASAuthorizationSingleSignOnRequest 

Class

# ASAuthorizationSingleSignOnRequest

An OpenID authorization request that provides single sign-on (SSO) functionality.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
class ASAuthorizationSingleSignOnRequest
```

## Topics

### Setting Options

var isUserInterfaceEnabled: Bool

var authorizationOptions: [URLQueryItem]

Options that control the authorization process.

## Relationships

### Inherits From

- ASAuthorizationOpenIDRequest

### Conforms To

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

### Creating Authorization Requests

var canPerformAuthorization: Bool

A Boolean value that indicates if the provider is capable of performing authorization within a given configuration.

func createRequest() -> ASAuthorizationSingleSignOnRequest

Creates a single sign-on (SSO) authorization request.

class ASAuthorizationOpenIDRequest

An OpenID authorization request.


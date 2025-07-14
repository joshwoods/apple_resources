

- Authentication Services
-  ASAuthorizationOpenIDRequest 

Class

# ASAuthorizationOpenIDRequest

An OpenID authorization request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class ASAuthorizationOpenIDRequest
```

## Topics

### Setting the Operation

var requestedOperation: ASAuthorization.OpenIDOperation

The OpenID authentication operation you want this request to perform.

struct OpenIDOperation

The kinds of operations that you can perform with OpenID authentication.

### Setting the Scope

var requestedScopes: [ASAuthorization.Scope]?

The contact information to be requested from the user during authentication.

struct Scope

The kinds of contact information that can be requested from the user.

### Setting the State

var state: String?

Data that’s returned to you unmodified in the corresponding credential after a successful authentication.

### Setting the Nonce

var nonce: String?

A string value to pass to the identity provider.

## Relationships

### Inherits From

- ASAuthorizationRequest

### Inherited By

- ASAuthorizationAppleIDRequest
- ASAuthorizationSingleSignOnRequest

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

### Creating Requests

func createRequest() -> ASAuthorizationAppleIDRequest

Creates a new Apple ID authorization request.

class ASAuthorizationAppleIDRequest

An OpenID authorization request that relies on the user’s Apple ID.


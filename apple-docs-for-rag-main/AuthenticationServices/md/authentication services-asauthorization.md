

- Authentication Services
-  ASAuthorization 

Class

# ASAuthorization

The encapsulation of a successful authorization by a controller.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class ASAuthorization
```

## Topics

### Getting the Provider

var provider: any ASAuthorizationProvider

The provider that created the request that resulted in the successful authorization.

### Getting the Credential

var credential: any ASAuthorizationCredential

Information provided about a user after successful authentication.

protocol ASAuthorizationCredential

An interface that all credentials share.

### Characterizing an Authorization

struct Scope

The kinds of contact information that can be requested from the user.

struct OpenIDOperation

The kinds of operations that you can perform with OpenID authentication.

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
- Sendable

## See Also

### Handling Successful Authorization

func authorizationController(ASAuthorizationController, didCompleteWithCustomMethod: ASAuthorizationCustomMethod)

Informs the delegate when authorization completes, and specifies the custom method the user selected.

func authorizationController(controller: ASAuthorizationController, didCompleteWithAuthorization: ASAuthorization)

Tells the delegate when authorization completes successfully.


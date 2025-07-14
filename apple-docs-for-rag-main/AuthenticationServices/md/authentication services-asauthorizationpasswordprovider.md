

- Authentication Services
-  ASAuthorizationPasswordProvider 

Class

# ASAuthorizationPasswordProvider

A mechanism for generating requests to perform keychain credential sharing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 6.0+

``` source
class ASAuthorizationPasswordProvider
```

## Topics

### Creating Requests

func createRequest() -> ASAuthorizationPasswordRequest

Creates a new password authorization request.

class ASAuthorizationPasswordRequest

An authorization request that uses credentials stored in the keychain.

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

### Passwords

Password AutoFill

Streamline your app’s login and onboarding procedures.

class ASPasswordCredential

A password credential.


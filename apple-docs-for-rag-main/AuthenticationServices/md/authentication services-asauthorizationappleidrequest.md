

- Authentication Services
-  ASAuthorizationAppleIDRequest 

Class

# ASAuthorizationAppleIDRequest

An OpenID authorization request that relies on the user’s Apple ID.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class ASAuthorizationAppleIDRequest
```

## Topics

### Setting the User

var user: String?

An identifier associated with the user’s Apple ID.

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

### Creating Requests

func createRequest() -> ASAuthorizationAppleIDRequest

Creates a new Apple ID authorization request.

class ASAuthorizationOpenIDRequest

An OpenID authorization request.


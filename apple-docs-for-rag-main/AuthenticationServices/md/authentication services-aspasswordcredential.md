

- Authentication Services
-  ASPasswordCredential 

Class

# ASPasswordCredential

A password credential.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 6.0+

``` source
class ASPasswordCredential
```

## Topics

### Creating a credential

init(user: String, password: String)

Initializes a password credential.

### Accessing the username and password

var user: String

The user for a password credential object.

var password: String

The password for a password credential object.

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

### Passwords

Password AutoFill

Streamline your app’s login and onboarding procedures.

class ASAuthorizationPasswordProvider

A mechanism for generating requests to perform keychain credential sharing.


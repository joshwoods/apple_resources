

- Local Authentication
-  LAAuthenticationRequirement 

Class

# LAAuthenticationRequirement

A set of requirements that protect a right.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class LAAuthenticationRequirement
```

## Topics

### Specifying authentication requirements

class var `default`: LAAuthenticationRequirement

The requirement that requires user authentication.

class var biometry: LAAuthenticationRequirement

The requirement that requires biometric authentication.

class var biometryCurrentSet: LAAuthenticationRequirement

The requirement that requires user authentication with the current set of biometrics.

class func biometry(fallback: LABiometryFallbackRequirement) -> Self

Creates a requirement that requires biometric authentication or a fallback requirement that you specify.

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

### Requirements

class LABiometryFallbackRequirement

A set of requirements to fall back on if biometrics aren’t present.


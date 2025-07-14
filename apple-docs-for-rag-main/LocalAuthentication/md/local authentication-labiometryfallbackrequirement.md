

- Local Authentication
-  LABiometryFallbackRequirement 

Class

# LABiometryFallbackRequirement

A set of requirements to fall back on if biometrics aren’t present.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class LABiometryFallbackRequirement
```

## Topics

### Specifying biometric fallback requirements

class var `default`: LABiometryFallbackRequirement

The default biometric fallback requirement.

class var devicePasscode: LABiometryFallbackRequirement

The fallback requirement that requires entering the device passcode.

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

class LAAuthenticationRequirement

A set of requirements that protect a right.


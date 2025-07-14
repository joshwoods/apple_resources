

- Local Authentication
- LAAuthenticationRequirement
-  default 

Type Property

# default

The requirement that requires user authentication.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class var `default`: LAAuthenticationRequirement { get }
```

## See Also

### Specifying authentication requirements

class var biometry: LAAuthenticationRequirement

The requirement that requires biometric authentication.

class var biometryCurrentSet: LAAuthenticationRequirement

The requirement that requires user authentication with the current set of biometrics.

class func biometry(fallback: LABiometryFallbackRequirement) -> Self

Creates a requirement that requires biometric authentication or a fallback requirement that you specify.


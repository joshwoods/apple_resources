

- Local Authentication
- LAAuthenticationRequirement
-  biometry 

Type Property

# biometry

The requirement that requires biometric authentication.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class var biometry: LAAuthenticationRequirement { get }
```

## Discussion

Authorizations with this requirement fail when biometrics aren’t available on the current device or there aren’t any enrolled biometrics on the current device.

## See Also

### Specifying authentication requirements

class var `default`: LAAuthenticationRequirement

The requirement that requires user authentication.

class var biometryCurrentSet: LAAuthenticationRequirement

The requirement that requires user authentication with the current set of biometrics.

class func biometry(fallback: LABiometryFallbackRequirement) -> Self

Creates a requirement that requires biometric authentication or a fallback requirement that you specify.


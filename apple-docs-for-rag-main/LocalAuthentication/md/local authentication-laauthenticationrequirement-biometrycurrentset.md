

- Local Authentication
- LAAuthenticationRequirement
-  biometryCurrentSet 

Type Property

# biometryCurrentSet

The requirement that requires user authentication with the current set of biometrics.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class var biometryCurrentSet: LAAuthenticationRequirement { get }
```

## Discussion

Authorizations with this requirement fail when:

- Biometrics aren’t available on the current device.

- There aren’t any enrolled biometrics on the current device.

- There’s a change in enrolled biometrics on the current device. For example, adding a new finger to Touch ID changes the set of enrolled biometrics.

## See Also

### Specifying authentication requirements

class var `default`: LAAuthenticationRequirement

The requirement that requires user authentication.

class var biometry: LAAuthenticationRequirement

The requirement that requires biometric authentication.

class func biometry(fallback: LABiometryFallbackRequirement) -> Self

Creates a requirement that requires biometric authentication or a fallback requirement that you specify.


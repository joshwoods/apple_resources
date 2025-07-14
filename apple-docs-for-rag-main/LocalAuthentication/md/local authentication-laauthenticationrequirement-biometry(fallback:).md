

- Local Authentication
- LAAuthenticationRequirement
-  biometry(fallback:) 

Type Method

# biometry(fallback:)

Creates a requirement that requires biometric authentication or a fallback requirement that you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class func biometry(fallback: LABiometryFallbackRequirement) -> Self
```

## Parameters 

`fallback`  

A requirement to use a fallback if biometric authentication fails or is unavailable, or if the user prefers not to use biometric authentication.

## Return Value

Returns a requirement that requires biometric authentication or a fallback requirement that you specify.

## See Also

### Specifying authentication requirements

class var `default`: LAAuthenticationRequirement

The requirement that requires user authentication.

class var biometry: LAAuthenticationRequirement

The requirement that requires biometric authentication.

class var biometryCurrentSet: LAAuthenticationRequirement

The requirement that requires user authentication with the current set of biometrics.


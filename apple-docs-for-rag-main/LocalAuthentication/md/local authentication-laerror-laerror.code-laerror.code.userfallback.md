

- Local Authentication
- LAError
- LAError.Code
-  LAError.Code.userFallback 

Case

# LAError.Code.userFallback

The user tapped the fallback button in the authentication dialog, but no fallback is available for the authentication policy.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 3.0+

``` source
case userFallback
```

## See Also

### Other errors

case authenticationFailed

The user failed to provide valid credentials.

case invalidContext

The context was previously invalidated.

case invalidDimensions

case notInteractive

Displaying the required authentication user interface is forbidden.

case passcodeNotSet

A passcode isn’t set on the device.

case watchNotAvailable

An attempt to authenticate with Apple Watch failed.

Deprecated


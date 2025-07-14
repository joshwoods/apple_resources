

- Local Authentication
- LAError
- LAError.Code
-  LAError.Code.invalidContext 

Case

# LAError.Code.invalidContext

The context was previously invalidated.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
case invalidContext
```

## Discussion

You invalidate a context by calling its invalidate() method.

## See Also

### Other errors

case authenticationFailed

The user failed to provide valid credentials.

case invalidDimensions

case notInteractive

Displaying the required authentication user interface is forbidden.

case passcodeNotSet

A passcode isn’t set on the device.

case userFallback

The user tapped the fallback button in the authentication dialog, but no fallback is available for the authentication policy.

case watchNotAvailable

An attempt to authenticate with Apple Watch failed.

Deprecated


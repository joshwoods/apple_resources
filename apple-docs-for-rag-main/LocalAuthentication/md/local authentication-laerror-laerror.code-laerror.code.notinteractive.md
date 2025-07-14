

- Local Authentication
- LAError
- LAError.Code
-  LAError.Code.notInteractive 

Case

# LAError.Code.notInteractive

Displaying the required authentication user interface is forbidden.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 3.0+

``` source
case notInteractive
```

## Discussion

Permit the display of the authentication UI by setting the interactionNotAllowed property to false.

## See Also

### Other errors

case authenticationFailed

The user failed to provide valid credentials.

case invalidContext

The context was previously invalidated.

case invalidDimensions

case passcodeNotSet

A passcode isn’t set on the device.

case userFallback

The user tapped the fallback button in the authentication dialog, but no fallback is available for the authentication policy.

case watchNotAvailable

An attempt to authenticate with Apple Watch failed.

Deprecated


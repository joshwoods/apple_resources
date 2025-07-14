

- Local Authentication
- LAError
- LAError.Code
-  LAError.Code.watchNotAvailable Deprecated

Case

# LAError.Code.watchNotAvailable

An attempt to authenticate with Apple Watch failed.

macOS 10.15–15.0Deprecated

``` source
case watchNotAvailable
```

## Discussion

You receive this error when the system fails to locate a nearby, paired Apple Watch running watchOS 6 or later while trying to authenticate using one of the watch authentication policies like LAPolicy.deviceOwnerAuthenticationWithWatch.

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

case userFallback

The user tapped the fallback button in the authentication dialog, but no fallback is available for the authentication policy.


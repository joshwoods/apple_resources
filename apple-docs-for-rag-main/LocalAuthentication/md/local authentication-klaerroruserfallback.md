

- Local Authentication
-  kLAErrorUserFallback 

Global Variable

# kLAErrorUserFallback

The user tapped the fallback button in the authentication dialog, but no fallback is available for the authentication policy.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+visionOS 1.0+watchOS 9.0+

``` source
var kLAErrorUserFallback: Int32 { get }
```

## See Also

### Supporting Constants

var kLAErrorDomain: String

The error domain used by LocalAuthentication.

var kLAErrorAppCancel: Int32

The app canceled authentication.

var kLAErrorSystemCancel: Int32

The system canceled authentication.

var kLAErrorUserCancel: Int32

The user tapped the cancel button in the authentication dialog.

var kLAErrorBiometryDisconnected: Int32

The device supports biometry only using a removable accessory, but the paired accessory isn’t connected.

var kLAErrorBiometryLockout: Int32

Biometry is locked because there were too many failed attempts.

var kLAErrorBiometryNotAvailable: Int32

Biometry is not available on the device.

var kLAErrorBiometryNotEnrolled: Int32

The user has no enrolled biometric identities.

var kLAErrorBiometryNotPaired: Int32

The device supports biometry only using a removable accessory, but no accessory is paired.

var kLAErrorTouchIDLockout: Int32

Touch ID is locked because there were too many failed attempts.

var kLAErrorTouchIDNotAvailable: Int32

Touch ID is not available on the device.

var kLAErrorTouchIDNotEnrolled: Int32

The user has no enrolled Touch ID fingers.

var kLAErrorAuthenticationFailed: Int32

The user failed to provide valid credentials.

var kLAErrorInvalidContext: Int32

The context was previously invalidated.

var kLAErrorInvalidDimensions: Int32




- Local Authentication
- LAError
-  touchIDNotEnrolled Deprecated

Type Property

# touchIDNotEnrolled

The user has no enrolled Touch ID fingers.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.13DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–4.0Deprecated

``` source
static var touchIDNotEnrolled: LAError.Code { get }
```

Deprecated

Use biometryNotEnrolled instead.

## See Also

### Error Codes

static var appCancel: LAError.Code

The app canceled authentication.

static var systemCancel: LAError.Code

The system canceled authentication.

static var userCancel: LAError.Code

The user tapped the cancel button in the authentication dialog.

static var biometryDisconnected: LAError.Code

The device supports biometry only using a removable accessory, but the paired accessory isn’t connected.

static var biometryLockout: LAError.Code

Biometry is locked because there were too many failed attempts.

static var biometryNotAvailable: LAError.Code

Biometry is not available on the device.

static var biometryNotEnrolled: LAError.Code

The user has no enrolled biometric identities.

static var biometryNotPaired: LAError.Code

The device supports biometry only using a removable accessory, but no accessory is paired.

static var touchIDLockout: LAError.Code

Touch ID is locked because there were too many failed attempts.

Deprecated

static var touchIDNotAvailable: LAError.Code

Touch ID is not available on the device.

Deprecated

static var authenticationFailed: LAError.Code

The user failed to provide valid credentials.

static var invalidContext: LAError.Code

The context was previously invalidated.

static var invalidDimensions: LAError.Code

static var notInteractive: LAError.Code

Displaying the required authentication user interface is forbidden.

static var passcodeNotSet: LAError.Code

A passcode isn’t set on the device.


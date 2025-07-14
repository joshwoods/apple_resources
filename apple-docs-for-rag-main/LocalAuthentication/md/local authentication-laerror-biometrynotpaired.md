

- Local Authentication
- LAError
-  biometryNotPaired 

Type Property

# biometryNotPaired

The device supports biometry only using a removable accessory, but no accessory is paired.

macOS 11.2+

``` source
static var biometryNotPaired: LAError.Code { get }
```

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

static var touchIDLockout: LAError.Code

Touch ID is locked because there were too many failed attempts.

Deprecated

static var touchIDNotAvailable: LAError.Code

Touch ID is not available on the device.

Deprecated

static var touchIDNotEnrolled: LAError.Code

The user has no enrolled Touch ID fingers.

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


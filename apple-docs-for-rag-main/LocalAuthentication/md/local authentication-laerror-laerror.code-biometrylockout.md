

- Local Authentication
- LAError
- LAError.Code
-  biometryLockout 

Type Property

# biometryLockout

Biometry is locked because there were too many failed attempts.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
static var biometryLockout: LAError.Code { get }
```

## Discussion

A passcode is now required to unlock biometry. Try the LAPolicy.deviceOwnerAuthentication policy instead to allow use of a passcode.

## See Also

### Biometry failure

case biometryDisconnected

The device supports biometry only using a removable accessory, but the paired accessory isn’t connected.

static var biometryNotAvailable: LAError.Code

Biometry is not available on the device.

static var biometryNotEnrolled: LAError.Code

The user has no enrolled biometric identities.

case biometryNotPaired

The device supports biometry only using a removable accessory, but no accessory is paired.

case touchIDLockout

Touch ID is locked because there were too many failed attempts.

Deprecated

case touchIDNotAvailable

Touch ID is not available on the device.

Deprecated

case touchIDNotEnrolled

The user has no enrolled Touch ID fingers.

Deprecated


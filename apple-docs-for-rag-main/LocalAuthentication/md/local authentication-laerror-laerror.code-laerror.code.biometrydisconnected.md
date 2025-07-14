

- Local Authentication
- LAError
- LAError.Code
-  LAError.Code.biometryDisconnected 

Case

# LAError.Code.biometryDisconnected

The device supports biometry only using a removable accessory, but the paired accessory isn’t connected.

macOS 11.2+

``` source
case biometryDisconnected
```

## See Also

### Biometry failure

static var biometryLockout: LAError.Code

Biometry is locked because there were too many failed attempts.

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


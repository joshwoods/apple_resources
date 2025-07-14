

- Local Authentication
- LAError
- LAError.Code
-  biometryNotEnrolled 

Type Property

# biometryNotEnrolled

The user has no enrolled biometric identities.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
static var biometryNotEnrolled: LAError.Code { get }
```

## See Also

### Biometry failure

case biometryDisconnected

The device supports biometry only using a removable accessory, but the paired accessory isn’t connected.

static var biometryLockout: LAError.Code

Biometry is locked because there were too many failed attempts.

static var biometryNotAvailable: LAError.Code

Biometry is not available on the device.

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


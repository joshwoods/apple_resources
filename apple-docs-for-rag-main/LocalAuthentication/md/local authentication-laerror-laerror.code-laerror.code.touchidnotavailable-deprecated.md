

- Local Authentication
- LAError
- LAError.Code
-  LAError.Code.touchIDNotAvailable Deprecated

Case

# LAError.Code.touchIDNotAvailable

Touch ID is not available on the device.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.13DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–4.0Deprecated

``` source
case touchIDNotAvailable
```

Deprecated

Use biometryNotAvailable(Swift) and LAErrorBiometryNotAvailable (Objective-C) instead.

## See Also

### Biometry failure

case biometryDisconnected

The device supports biometry only using a removable accessory, but the paired accessory isn’t connected.

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

case touchIDNotEnrolled

The user has no enrolled Touch ID fingers.

Deprecated


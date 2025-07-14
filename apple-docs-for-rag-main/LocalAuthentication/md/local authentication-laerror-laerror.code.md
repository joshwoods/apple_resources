

- Local Authentication
- LAError
-  LAError.Code 

Enumeration

# LAError.Code

Errors issued by the LocalAuthentication framework.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 3.0+

``` source
enum Code
```

## Topics

### Cancellation

case appCancel

The app canceled authentication.

case systemCancel

The system canceled authentication.

case userCancel

The user tapped the cancel button in the authentication dialog.

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

case touchIDNotAvailable

Touch ID is not available on the device.

Deprecated

case touchIDNotEnrolled

The user has no enrolled Touch ID fingers.

Deprecated

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

case watchNotAvailable

An attempt to authenticate with Apple Watch failed.

Deprecated

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

var kLAErrorNotInteractive: Int32

Displaying the required authentication user interface is forbidden.

var kLAErrorPasscodeNotSet: Int32

A passcode isn’t set on the device.

var kLAErrorUserFallback: Int32

The user tapped the fallback button in the authentication dialog, but no fallback is available for the authentication policy.

var kLAErrorWatchNotAvailable: Int32

An attempt to authenticate with Apple Watch failed.

### Initializers

init?(rawValue: Int)

### Type Properties

static var companionNotAvailable: LAError.Code

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct LAError

Errors issued by the LocalAuthentication framework.

let LAErrorDomain: String

The error domain that the framework uses when issuing errors.


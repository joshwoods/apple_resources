

- Local Authentication
-  LAPolicy 

Enumeration

# LAPolicy

The set of available local authentication policies.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 3.0+

``` source
enum LAPolicy
```

## Topics

### Policies

case deviceOwnerAuthenticationWithBiometrics

User authentication with biometry.

case deviceOwnerAuthenticationWithWatch

User authentication with Apple Watch.

Deprecated

case deviceOwnerAuthenticationWithBiometricsOrWatch

User authentication with either biometry or Apple Watch.

Deprecated

case deviceOwnerAuthentication

User authentication with biometry, Apple Watch, or the device passcode.

case deviceOwnerAuthenticationWithWristDetection

User authentication with wrist detection on watchOS.

### Policy Constants

var kLAPolicyDeviceOwnerAuthenticationWithBiometrics: Int32

User authentication with biometry.

var kLAPolicyDeviceOwnerAuthenticationWithWatch: Int32

User authentication with Apple Watch.

var kLAPolicyDeviceOwnerAuthenticationWithBiometricsOrWatch: Int32

User authentication with either biometry or Apple Watch.

var kLAPolicyDeviceOwnerAuthentication: Int32

User authentication with either biometry or the device passcode.

var kLAPolicyDeviceOwnerAuthenticationWithWristDetection: Int32

User authentication with wrist detection on watchOS.

### Initializers

init?(rawValue: Int)

### Type Properties

static var deviceOwnerAuthenticationWithBiometricsOrCompanion: LAPolicy

Device owner will be authenticated by biometry or a companion device e.g. Watch, Mac, etc.

static var deviceOwnerAuthenticationWithCompanion: LAPolicy

Device owner will be authenticated by a companion device e.g. Watch, Mac, etc.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Checking availability

func canEvaluatePolicy(LAPolicy, error: NSErrorPointer) -> Bool

Assesses whether authentication can proceed for a given policy.

var biometryType: LABiometryType

The type of biometric authentication supported by the device.

enum LABiometryType

The set of available biometric authentication types.




- Local Authentication
-  LABiometryType 

Enumeration

# LABiometryType

The set of available biometric authentication types.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13.2+visionOS 1.0+watchOS 11.0+

``` source
enum LABiometryType
```

## Topics

### Types

case none

No biometry type is supported.

case faceID

The device supports Face ID.

case touchID

The device supports Touch ID.

case opticID

The device supports Optic ID.

### Legacy Types

static var LABiometryNone: LABiometryType

No biometry type is supported.

Deprecated

### Initializers

init?(rawValue: Int)

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

enum LAPolicy

The set of available local authentication policies.

var biometryType: LABiometryType

The type of biometric authentication supported by the device.


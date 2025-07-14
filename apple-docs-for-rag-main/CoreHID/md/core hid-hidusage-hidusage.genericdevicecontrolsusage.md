

- Core HID
- HIDUsage
-  HIDUsage.GenericDeviceControlsUsage 

Enumeration

# HIDUsage.GenericDeviceControlsUsage

macOS 15.0+

``` source
enum GenericDeviceControlsUsage
```

## Topics

### Enumeration Cases

case backgroundOrNonuserControls

case batteryStrength

case bothHands

case discoverWirelessControl

case eitherHand

case gripPoseOffset

case handedness

case hardwareVersion

case leftHand

case major

case minor

case pointerPoseOffset

case protocolVersion

case revision

case rfSignalStrength

case rightHand

case securityCodeCharacterEntered

case securityCodeCharacterErased

case securityCodeCleared

case sequenceID

case sequenceIDReset

case softwareVersion

case wirelessChannel

case wirelessID

### Initializers

init?(rawValue: UInt16)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: UInt16

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let page: UInt16

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable


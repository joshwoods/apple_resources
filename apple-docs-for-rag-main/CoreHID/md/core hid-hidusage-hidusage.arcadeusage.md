

- Core HID
- HIDUsage
-  HIDUsage.ArcadeUsage 

Enumeration

# HIDUsage.ArcadeUsage

macOS 15.0+

``` source
enum ArcadeUsage
```

## Topics

### Enumeration Cases

case alarmInput

case coinDoor

case coinDoorCounter

case coinDoorLockout

case coinDoorTest

case coinDrawerDropCount

case coinDrawerService

case coinDrawerStart

case coinDrawerTilt

case extendedOpticalInputState

case generalPurposeAnalogInputState

case generalPurposeDigitalInputState

case generalPurposeDigitalOutputState

case generalPurposeIOCard

case generalPurposeOpticalInputState

case ioDirectionMapping

case numberOfCoinDoors

case pinPadCommand

case pinPadInputState

case pinPadOutput

case pinPadStatus

case setIODirectionMapping

case watchdogAction

case watchdogReboot

case watchdogRestart

case watchdogTimeout

case watchdogTimer

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


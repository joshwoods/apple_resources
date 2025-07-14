

- HomeKit
-  HMCharacteristicValueVolumeControlType 

Enumeration

# HMCharacteristicValueVolumeControlType

Values for the type of volume control.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
enum HMCharacteristicValueVolumeControlType
```

## Topics

### Volume types

case absolute

The volume sets to a specific level.

case none

The device doesn’t have volume control functionality.

case relative

The volume adjusts incrementally, without taking the current level into consideration.

case relativeWithCurrent

The volume adjusts incrementally, relative to current level.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable


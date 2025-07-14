

- Core HID
- HIDUsage
-  HIDUsage.SportControlsUsage 

Enumeration

# HIDUsage.SportControlsUsage

macOS 15.0+

``` source
enum SportControlsUsage
```

## Topics

### Enumeration Cases

case baseballBat

case eightIron

case elevenIron

case fiveIron

case fiveWood

case fourIron

case golfClub

case loftWedge

case nineIron

case nineWood

case oar

case oneIron

case oneWood

case powerWedge

case putter

case rate

case rowingMachine

case sandWedge

case sevenIron

case sevenWood

case sixIron

case slope

case stickFaceAngle

case stickFollowThrough

case stickHeelOrToe

case stickHeight

case stickSpeed

case stickTempo

case stickType

case tenIron

case threeIron

case threeWood

case treadmill

case twoIron

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


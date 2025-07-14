

- Core HID
- HIDUsage
-  HIDUsage.LightingAndIlluminationUsage 

Enumeration

# HIDUsage.LightingAndIlluminationUsage

macOS 15.0+

``` source
enum LightingAndIlluminationUsage
```

## Topics

### Enumeration Cases

case autonomousMode

case blueLevelCount

case blueUpdateChannel

case boundingBoxDepthInMicrometers

case boundingBoxHeightInMicrometers

case boundingBoxWidthInMicrometers

case greenLevelCount

case greenUpdateChannel

case inputBinding

case intensityLevelCount

case intensityUpdateChannel

case isProgrammable

case lampArray

case lampArrayAttributesReport

case lampArrayControlReport

case lampArrayKind

case lampAttributesRequestReport

case lampAttributesResponseReport

case lampCount

case lampId

case lampIdEnd

case lampIdStart

case lampMultiUpdateReport

case lampPurposes

case lampRangeUpdateReport

case lampUpdateFlags

case minUpdateIntervalInMicroseconds

case positionXInMicrometers

case positionYInMicrometers

case positionZInMicrometers

case redLevelCount

case redUpdateChannel

case updateLatencyInMicroseconds

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




- Core HID
- HIDUsage
-  HIDUsage.MagneticStripeReaderUsage 

Enumeration

# HIDUsage.MagneticStripeReaderUsage

macOS 15.0+

``` source
enum MagneticStripeReaderUsage
```

## Topics

### Enumeration Cases

case msrDeviceReadOnly

case track1Data

case track1Length

case track2Data

case track2Length

case track3Data

case track3Length

case trackData

case trackJISData

case trackJISLength

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


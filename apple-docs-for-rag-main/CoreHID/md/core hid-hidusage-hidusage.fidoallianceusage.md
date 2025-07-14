

- Core HID
- HIDUsage
-  HIDUsage.FIDOAllianceUsage 

Enumeration

# HIDUsage.FIDOAllianceUsage

macOS 15.0+

``` source
enum FIDOAllianceUsage
```

## Topics

### Enumeration Cases

case inputReportData

case outputReportData

case u2fAuthenticatorDevice

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


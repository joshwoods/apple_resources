

- Core HID
- HIDUsage
-  HIDUsage.CameraControlUsage 

Enumeration

# HIDUsage.CameraControlUsage

macOS 15.0+

``` source
enum CameraControlUsage
```

## Topics

### Enumeration Cases

case cameraAutoFocus

case cameraShutter

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


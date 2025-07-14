

- Core HID
- HIDUsage
-  HIDUsage.VRControlsUsage 

Enumeration

# HIDUsage.VRControlsUsage

macOS 15.0+

``` source
enum VRControlsUsage
```

## Topics

### Enumeration Cases

case animatronicDevice

case belt

case bodySuit

case displayEnable

case flexor

case glove

case handTracker

case headMountedDisplay

case headTracker

case oculometer

case stereoEnable

case vest

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


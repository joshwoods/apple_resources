

- DeviceActivity
- DeviceActivityData
- DeviceActivityData.Device
-  DeviceActivityData.Device.Model 

Enumeration

# DeviceActivityData.Device.Model

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
enum Model
```

## Topics

### Enumeration Cases

case iPad

The device is an iPad.

case iPhone

The device is an iPhone.

case iPod

The device is an iPod.

case mac

The device is a Mac.

### Initializers

init?(rawValue: Int)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: Int

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable




- DeviceActivity
- DeviceActivityData
-  DeviceActivityData.Device 

Structure

# DeviceActivityData.Device

A device for which to report activity data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct Device
```

## Topics

### Operators

static func == (DeviceActivityData.Device, DeviceActivityData.Device) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

var model: DeviceActivityData.Device.Model

The model of the device.

var name: String?

The name of the device set by the user.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Enumerations

enum Model

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

